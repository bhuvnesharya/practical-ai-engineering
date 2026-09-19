# Agentic AI System Design, Part 2: Memory, Auth, PII, Evals, and Observability

**Watch:** add the YouTube URL · 2026-09-19  
**Series:** [Agentic AI System Design](../series/agentic-ai-system-design.md)

Status: URL pending — paste the public watch link when the video is up.

## In this video

- Priya comes back: load case RF-2291 (memory), then refresh Payments
- “All orders of mine” needs authentication — a signed-in customer id
- FB-10390 is Sana Khan’s: authorization refuses the shipment lookup. The model is not the security boundary
- A card number in chat is masked before the coordinator or the model can see it
- Company LLM first; a third-party model only gets a clean question
- Golden set: replay a new prompt, score a system that can answer differently each time
- Traces, monitoring, and a daily cost cap
- Close: the production map of the same Help chat

## Learn

- [Security & guardrails](../learn/security-guardrails/)
- [Data & knowledge](../learn/data-knowledge/)

## Practice

- [Brass Vernier](../practice/brass-vernier/README.md) — security and data domains fill in as those scenarios are catalogued

## Teaching world

- [Fictional Bazaar](./worlds/fictional-bazaar.md)

## Next

- Watch [Part 1](./agentic-ai-system-design-part-1.md) first if the coordinator, HITL, or retrieval blocks are new.
