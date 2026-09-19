# Agentic AI System Design, Part 2: Memory, Auth, PII, Evals, and Observability

**Watch:** add the YouTube URL · 2026-09-19  
**Series:** [Agentic AI System Design](../series/agentic-ai-system-design.md)  
**Studio:** [Part 2 deck](https://github.com/bhuvnesharya/agentic-ai-system-design/tree/main/presentations/agentic-ai-system-design-part-2)

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

## Practice

- Insight Veda: https://insightveda.com/

## Scenario

- [Fictional Bazaar](../scenarios/fictional-bazaar.md)

## Diagrams

- Production close diagram lives in the studio repo (`assets/diagrams/p2-08-production.svg`)

## Next

- Watch [Part 1](./agentic-ai-system-design-part-1.md) first if the coordinator, HITL, or RAG blocks are new.
