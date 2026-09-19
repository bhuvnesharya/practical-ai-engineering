---
name: maintain-hub
description: >-
  Maintains the public Practical AI Engineering map: YouTube pages, Insight Veda
  Learn chapter rows, Practice folio pages (domain links only), and CONNECT.
  Use when a chapter or folio ships, a video ships, or the user asks to update
  this repository. Do not create one file per practice scenario.
---

# Maintain the hub

Read [templates.md](templates.md) and [conventions.md](conventions.md).

## Shape

```
learn/<domain-id>.md          chapter name + /chapters?chapter=id
practice/<folio-id>.md        five rows: /scenarios?set=folio&domain=id
videos/ + series/             YouTube
```

Domain ids (must match Insight Veda): `agentic-architecture`, `data-knowledge`, `tools-integrations`, `prompting-output`, `security-guardrails`.

## Decide the artifact

| User intent | Do this |
| --- | --- |
| New chapter (usual: one per new folio, in a domain) | Add a row to `learn/<domain>.md`. Update What’s new. |
| New folio | Add `practice/<folio-id>.md` with five domain links. List it on `practice/README.md` (live first). Add the matching chapter row(s). |
| New YouTube video | `videos/<slug>.md` + series + What’s new. Point Learn/Practice at chapter and folio **URLs**, not private decks. |
| YouTube world | `videos/worlds/<slug>.md` |
| Profile change | `CONNECT.md` |

**Never** add `practice/.../01-some-case.md`. The site already lists the five cases when you open `set` + `domain`.

## Insight Veda URLs

| What | Pattern |
| --- | --- |
| All chapters | `https://insightveda.com/chapters` |
| Domain chapters | `https://insightveda.com/chapters?domain=<domain-id>` |
| One chapter | `https://insightveda.com/chapters?chapter=<chapter-id>` |
| All sets | `https://insightveda.com/scenarios` |
| One folio | `https://insightveda.com/scenarios?set=<folio-id>` |
| Folio × domain | `https://insightveda.com/scenarios?set=<folio-id>&domain=<domain-id>` |

There is no `/learn` or `/practice` path. Do not invent them.

## Checks

- [ ] No per-scenario GitHub files
- [ ] No `/learn` or `/practice` links
- [ ] No private GitHub repos
- [ ] Chapter and folio ids copied from Insight Veda, not guessed
