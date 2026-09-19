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

Explain each step for a beginner. Then **Links** as `Title ([link](url))` — not the whole line as a hyperlink, not a brand name.

Public markdown is for readers. Maintainer rules live in CONTRIBUTING.md and `.cursor/skills/maintain-hub/`, not in the page body.

Roadmap pages: five steps of teaching. Point once, near the top, at the chapters list and the papers list. Do not repeat those two links under every step.
