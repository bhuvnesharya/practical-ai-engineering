# Hub conventions

## What this repo is

A map of Bhuvnesh Arya's teaching: Practical AI Engineering. Developers land here from YouTube and go to a video page, an Insight Veda case, a scenario, or the diagram studio.

Studio (slides, SVG, mockups): https://github.com/bhuvnesharya/agentic-ai-system-design  
Practice and written lessons: https://insightveda.com/

## Naming

- Videos: `videos/<series>-part-n.md` or `videos/<problem-slug>.md`
- Series: `series/<series-slug>.md`
- Scenarios: company or product story, e.g. `scenarios/fictional-bazaar.md`
- Patterns: the failure they fix, e.g. `patterns/authorization-is-not-the-model.md`

Never: `langgraph-2026.md`, `awesome-agents.md`.

## Voice

- Audience: developers shipping systems, not "architects only"
- One idea per sentence
- Problem → what we added → where it sits
- Fictional names stay fictional (Fictional Bazaar, Priya Iyer)

## README

Four doors only. What's new is the only weekly-moving block. Do not grow the README into a catalog.

## Published pages

Do not rewrite history on a shipped video page. Add:

```markdown
## Later

Part 2 added memory, auth, and evals on the same Help chat. See [Part 2](../videos/agentic-ai-system-design-part-2.md).
```

## Out of scope

Interview question banks, certification, other people's course lists, monthly paper posts, tool roundups.
