---
name: maintain-hub
description: >-
  Maintains the public Practical AI Engineering map: YouTube video pages,
  Insight Veda chapter rows, folio pages, system-design topics, and five-step
  roadmaps with SVG diagrams. Use when a chapter, folio, video, topic, or
  roadmap ships. Do not create per-scenario files or a worlds folder.
---

# Maintain the hub

Read [templates.md](templates.md) and [conventions.md](conventions.md).

## Shape

```
learn/<domain-id>.md
practice/<folio-id>.md
topics/<topic-slug>.md          one video or several parts (MCP, RAG, Agentic, ...)
videos/<slug>.md
roadmaps/<name>.md              Step 1-5 + img/<name>.svg (1920x1080)
```

Domain ids: `agentic-architecture`, `data-knowledge`, `tools-integrations`, `prompting-output`, `security-guardrails`.

## Decide the artifact

| User intent | Do this |
| --- | --- |
| New chapter | Row on `learn/<domain>.md` |
| New folio | `practice/<folio>.md` with five domain links |
| New YouTube video | `videos/<slug>.md` + `topics/<slug>.md` (create or append). Optional: link a roadmap |
| New roadmap | `roadmaps/<name>.md` Steps 1-5. Beginner explanation, then public **Links**. GitHub SVG from `library/github-visuals.md`. Insight Veda only as `/chapters?domain=`. No Practice. No per-chapter URLs. |
| Profile change | `CONNECT.md` |

Never: per-scenario files, `/learn` or `/practice` site paths, private GitHub, `videos/worlds/`.

## Insight Veda URLs

| What | Pattern |
| --- | --- |
| All chapters | `https://insightveda.com/chapters` |
| Domain chapters | `https://insightveda.com/chapters?domain=<id>` |
| One chapter | `https://insightveda.com/chapters?chapter=<id>` |
| One folio | `https://insightveda.com/scenarios?set=<id>` |
| Folio × domain | `https://insightveda.com/scenarios?set=<id>&domain=<id>` |

## Roadmap diagrams

GitHub only: [library/github-visuals.md](../../../library/github-visuals.md) (paper, ink, rust accent, ~1200x640). Do not reuse YouTube navy slides. Do not put GitHub SVGs on OBS.

## Checks

- [ ] No per-scenario files, no worlds folder
- [ ] Topics, not “series required”
- [ ] Roadmaps are five steps; RAG style: explain, then links; domain not chapter; no Practice
- [ ] No private repos
