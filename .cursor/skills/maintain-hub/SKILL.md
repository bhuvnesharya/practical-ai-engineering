---
name: maintain-hub
description: >-
  Creates and maintains the public Practical AI Engineering map: YouTube video
  pages, Insight Veda Learn chapters (by domain), Practice folios and scenarios,
  and CONNECT links. Use when a new chapter, folio, scenario, or video ships, or
  when the user asks to update this repository.
---

# Maintain the hub

Read [templates.md](templates.md) before writing a file. Read [conventions.md](conventions.md) for the Insight Veda tree and the public-only rule.

## How the public map is shaped

```
YouTube          series/ + videos/ + videos/worlds/
Insight Veda     learn/<domain>/<nn>-<slug>.md     (chapters grow inside a domain)
                 practice/<folio>/<domain>/<nn>-<slug>.md
```

Learn and Practice share the **same five domains**. A folio is the named pack of 25 scenarios (five per domain). New chapters append `02`, `03` in that domain folder. New practice work usually lands as a **new folio**, while older folios stay listed for practice.

## Decide the artifact

| User intent | Create / update |
| --- | --- |
| New YouTube video | `videos/<slug>.md`, series card, `videos/README.md`, README What’s new |
| New YouTube series | `series/<slug>.md` |
| YouTube teaching world (Priya, …) | `videos/worlds/<slug>.md` — not an Insight Veda folio |
| New Learn domain (rare) | `learn/<domain>/README.md` + row on `learn/README.md` |
| New chapter in an existing domain | `learn/<domain>/<nn>-<slug>.md`, update that domain README + `learn/README.md` counts |
| New Practice folio | `practice/<folio>/README.md` + five domain folders, live folio listed first on `practice/README.md` |
| New scenario | `practice/<folio>/<domain>/<nn>-<slug>.md`, bump folio and domain counts |
| Profile / site URL | `CONNECT.md` only |

Slug: lowercase, hyphens. Folio names stay human in the title (`Brass Vernier`) and kebab in the path (`brass-vernier`).

## Workflow

1. Pick the row in the table.
2. Copy the template. Fill `TODO`.
3. **Insight Veda Open link:** prefer `https://insightveda.com/learn` or `https://insightveda.com/practice` plus the on-site path (Domain → Chapter, or Folio → Domain → Scenario). Add a deep URL only when the user gives a public permalink.
4. **YouTube Watch link:** real `youtube.com/watch` only. Otherwise `Status: URL pending` and keep it off any “watch now” promo.
5. Cross-link: chapter ↔ same-domain scenarios in the **live** folio; video ↔ learn domain and/or folio.
6. Prepend README **What’s new** (newest first, max 8 bullets). Date `YYYY-MM-DD`.
7. Never link a private GitHub repo. Never paste the full Insight Veda lesson or the full scenario prompt.

## Checks before you stop

- [ ] Template headings used
- [ ] No private studio / slides / SVG repo URLs
- [ ] No full lesson or case dump
- [ ] Parent README tables/counts updated
- [ ] CONNECT.md is public URLs only
