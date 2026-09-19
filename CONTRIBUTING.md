# Contributing

This repo is a **public map** for people who want to design AI systems that actually run. You do not need to know the maintainer or any product brand. PRs that make the map more useful are welcome. PRs that turn it into a blogroll are not.

## What we want

| Kind | Example | How |
| --- | --- | --- |
| Paper for a table | A RAG eval paper with an arXiv link | Add a row to `references/rag-papers.md` |
| Lesson for a roadmap | A new public chapter on chunking, retrieval, … | Add a bullet under the matching step in `references/rag-chapters.md` (not on `roadmaps/rag.md`) |
| Fix | Broken URL, typo | PR with a one-line why |

## What we will usually close

- Personal or company blogs (`someone.com/blog/my-rag-stack`). They age badly, they are hard to vet, and they turn the roadmap into SEO.
- “Also read my newsletter.”
- A new arXiv paper that does not change how you **build** (another incremental reranker, another tiny benchmark).
- Duplicate of a row that is already here.

Vendor tutorials (Pinecone, LangChain, LlamaIndex) are not the default. Prefer a paper or a self-contained explanation. Keep a vendor doc only when it is still the clearest public write-up for that step.

## How to add a paper

1. Open `references/rag-papers.md` (or the matching table when other topics get one).
2. Add **year, title, one sentence why it belongs, arXiv (or DOI) link**.
3. Put it where a reader should meet it, not automatically at the top.
4. In the PR, say in one sentence: what primitive or measurement this paper adds.

Maintainers may rewrite the one-liner, move the row, or reject it. The table stays short on purpose.

## How to add a lesson to a roadmap

Do not add new chapter URLs to `roadmaps/rag.md`. That page stays five steps.

1. Open `references/rag-chapters.md`.
2. Add `Topic title ([link](url))` under the matching step.
3. Title is the topic, not a brand.

## Review bar

A maintainer will ask: would a stranger who never heard of us still click this, and would they learn the step? If the only reason to click is “our site,” it does not belong on the roadmap.
