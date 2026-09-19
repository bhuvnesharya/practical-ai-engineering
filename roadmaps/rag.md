# RAG roadmap

A language model does not contain your return policy, your runbooks, or last week’s order notes. If you paste the whole handbook into the prompt, you hit context limits and still miss the clause that matters.

RAG (retrieval-augmented generation) is the simple fix: **find a few relevant passages first, then ask the model to answer from those passages.**

![RAG roadmap](img/rag.svg)

```
question --> retrieve passages --> add them to the prompt --> model --> answer from those passages
```

Work the steps in order. A better embedding model will not save a bad chunk.

Lessons for these steps: [RAG chapters](../references/rag-chapters.md). Papers: [RAG papers](../references/rag-papers.md).

## Step 1 — Chunk

Your source is a PDF, a wiki, or a policy doc. The index cannot store it as one blob. You split it into **chunks**: pieces small enough to search, large enough to still mean something.

If you cut mid-sentence, retrieval returns fragments. If a rule and its exception land in two chunks with no overlap, the model may see the rule and miss the exception. Overlap (repeating the last lines of chunk A at the start of chunk B) is a simple way to protect those boundaries.

There is no magic token size. Start from the questions people actually ask. If they need a short procedure, the chunk must hold that procedure.

**Links**

1. RAG chapters ([link](../references/rag-chapters.md#step-1-chunk))
2. RAG papers ([link](../references/rag-papers.md))

## Step 2 — Index

You store those chunks somewhere you can search: a vector index, a keyword index, or both. Each record should carry **metadata** you can read when an answer is wrong: source file, section title, date.

If you cannot say “this sentence came from Returns, page 4,” you cannot debug RAG. You will only argue with the model.

**Links**

1. RAG chapters ([link](../references/rag-chapters.md#step-2-index))
2. RAG papers ([link](../references/rag-papers.md))

## Step 3 — Retrieve

At question time you do not load the corpus. You **search** and take the top passages. Vector search finds similar meaning. Keyword search finds exact names, ids, and clause numbers. Many production systems use both (hybrid), then keep the top few.

If the right clause is not in those hits, the model cannot honestly use it. Retrieval quality is the ceiling for answer quality.

**Links**

1. RAG chapters ([link](../references/rag-chapters.md#step-3-retrieve))
2. RAG papers ([link](../references/rag-papers.md))

## Step 4 — Ground

The model now sees the user question **plus** the retrieved text. The instruction is: answer from that text. If the passages do not contain the answer, say you do not know. Point at the source when you can.

This is the difference between “the model recalled a policy” and “the system showed the policy.” Guessing is not RAG.

**Links**

1. RAG chapters ([link](../references/rag-chapters.md#step-4-ground))
2. RAG papers ([link](../references/rag-papers.md))

## Step 5 — Harden

Before you add agentic retrieval or a graph index, ask three production questions:

1. **Access** — may this user see this chunk? Retrieval must follow the same rules as your files.
2. **Freshness** — is the index the current policy, or last quarter’s PDF?
3. **Eval** — for a small set of trusted questions, did we retrieve the right passage, and did the answer stay inside it?

If you cannot measure those, a smarter retriever will only fail faster.

**Links**

1. RAG chapters ([link](../references/rag-chapters.md#step-5-harden))
2. RAG papers ([link](../references/rag-papers.md))
