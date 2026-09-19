# GitHub visual system

Use this for diagrams that live on GitHub (`roadmaps/img/` and similar). Do **not** copy the YouTube deck (navy `#0B1220`, teal `#3D9B8F`, IBM Plex title cards, 1920x1080 OBS slides).

Those slides stay in the private studio. GitHub diagrams should look like a **print figure**: paper, ink, one accent.

## Tokens

| Token | Value | Use |
| --- | --- | --- |
| Paper | `#FAF7F2` | Background |
| Rule | `#E4DDD2` | Hairlines |
| Ink | `#1F1B16` | Titles |
| Quiet | `#6A6158` | Captions |
| Accent | `#9A4A2A` | Step numbers only |
| Type | `Georgia, Times New Roman, serif` | Titles |
| Type UI | `Segoe UI, Helvetica, sans-serif` | Small labels |

## Layout

- Wider than tall is fine, but not a 1080p title card. Prefer about **1200 x 640**.
- Five steps as a **horizontal spine**: numbered discs, short names, one connecting rule.
- No glow, no dashed “product” frames, no kicker in teal small-caps like the deck.
- ASCII-only text in SVG.

## After you draw

Embed with `![...](img/....svg)` on the roadmap page. If a YouTube video needs a diagram, rebuild it in the studio. Do not paste this SVG onto the OBS slide.
