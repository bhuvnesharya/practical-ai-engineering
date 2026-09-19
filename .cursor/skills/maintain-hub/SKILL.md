---
name: maintain-hub
description: >-
  Creates and maintains Practical AI Engineering hub artifacts: video pages,
  series cards, scenarios, README doors, and CONNECT links. Use when adding a
  YouTube video, Insight Veda lesson or case, a fictional scenario, a system
  pattern, or when the user asks to update this repository.
---

# Maintain the hub

This repository is a front door for developers. Keep it small, linked, and durable.

Read [templates.md](templates.md) before writing a new file. Read [conventions.md](conventions.md) if the change is a rename, a series, or a What's new edit.

## Decide the artifact

| User intent | Create / update |
| --- | --- |
| New YouTube video | `videos/<slug>.md`, series card, README What's new + Watch table |
| New series (no video yet) | `series/<slug>.md` only |
| Insight Veda lesson or case | Link it from the related video and series. Do not paste the lesson. |
| New story world | `scenarios/<slug>.md` |
| Pattern (HITL, PII masking, …) | `patterns/<problem-slug>.md` |
| Profile / site change | `CONNECT.md` |

Slug: lowercase, hyphens, no year, no product name unless it is the series (`agentic-ai-system-design-part-2`).

## Workflow

1. Identify the artifact type from the table.
2. Copy the matching template from [templates.md](templates.md).
3. Fill every `TODO`. Do not publish a Watch row without a real YouTube URL. If the URL is unknown, leave the page off the README Watch table and mark the page `Status: URL pending`.
4. Link sideways: video → series → scenario → studio repo and/or Insight Veda.
5. Prepend README **What's new** (newest first, max 8 bullets). Date as `YYYY-MM-DD`.
6. Do not add folders for courses, interviews, or research feeds.

## Checks before you stop

- [ ] New markdown uses a template heading set
- [ ] No copied SVG, HTML mockup, or full Insight Veda lesson
- [ ] README doors still match the four starts: Watch, Practice, Read, Diagrams
- [ ] CONNECT.md still has working `https://` URLs
