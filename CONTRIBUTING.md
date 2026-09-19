# Contributing

This repo is a **public map** for people who want to design AI systems that actually run. You do not need to know the maintainer or any product brand. PRs that make the map more useful are welcome. PRs that turn it into a blogroll are not.

## What we want

| Kind | Example | How |
| --- | --- | --- |
| Paper for a table | A RAG eval paper with an arXiv link | Add a row to `references/rag-papers.md` |
| Canonical doc | Original RAG paper, OWASP LLM Top 10 | Link it from the matching roadmap step |
| Fix | Broken URL, clearer step, typo | PR with a one-line why |
| New roadmap step resource | A *better* beginner explanation than what is there | Replace or put it **first** in that step’s list |

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

## How to add a link on a roadmap

Roadmaps teach in the markdown. Links are optional extras.

Format (text, then a short `(link)`):

```markdown
- Chunking and overlap ([link](https://...))
- RAG papers ([link](../references/rag-papers.md))
```

Do not wrap the whole sentence in the hyperlink. Do not label links with a product brand. Name the **topic** (what the reader gets).

If you wrote a public chapter that explains the step better than the current first link, that chapter can go first. Still title it as the topic, not as a brand.

## Review bar

A maintainer will ask: would a stranger who never heard of us still click this, and would they learn the step? If the only reason to click is “our site,” it does not belong on the roadmap.
