# Templates

## Learn domain and practice folio

Unchanged: chapter rows and five domain links. See existing `learn/` and `practice/` files.

## Topic (`topics/<slug>.md`)

```markdown
# TODO: topic title

One paragraph. Can be a single video.

## Videos

1. [TODO](../videos/TODO.md)

## Roadmap

[TODO](../roadmaps/TODO.md) if one exists

## Learn / Practice

- https://insightveda.com/chapters?domain=TODO
- https://insightveda.com/scenarios?set=TODO
```

## Video (`videos/<slug>.md`)

```markdown
# TODO: YouTube title

**Watch:** [TODO](https://www.youtube.com/watch?v=TODO) · YYYY-MM-DD  
**Topic:** [TODO](../topics/TODO.md)  
**Roadmap:** [TODO](../roadmaps/TODO.md)

## In this video

- TODO

## Learn

- [TODO](https://insightveda.com/chapters?chapter=TODO)

## Practice

- [TODO](https://insightveda.com/scenarios?set=TODO&domain=TODO)
```

## Roadmap (`roadmaps/<name>.md`)

Follow [library/github-visuals.md](../../../library/github-visuals.md) for the SVG. Do not copy YouTube deck colors.

Explain each step for a beginner. Then **Links** (public articles, papers, docs first). Insight Veda is optional and must be the **domain** (`/chapters?domain=`), never a single chapter and never Practice.

```markdown
# TODO title

Beginner intro. What problem this roadmap solves.

![TODO](img/TODO.svg)

## Step 1 — TODO

A few short paragraphs. What it is. What goes wrong if you skip it.

**Links**

- [Public resource](https://...)
- Insight Veda: [Domain name](https://insightveda.com/chapters?domain=TODO)
```

Five steps. See `roadmaps/rag.md` as the current example. Do not add Practice rows.
