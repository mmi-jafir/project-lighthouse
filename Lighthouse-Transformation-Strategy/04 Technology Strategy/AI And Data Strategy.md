# AI and Data Strategy
### Project Lighthouse — Knowledge Infrastructure Transformation

**Version:** 1.0
**Related:** `Platform And Ecosystem Strategy.md`, `../07 Decisions/003 AI Confidentiality Safeguard Scope.md`

---

## 1. Purpose of AI in This Transformation

AI (semantic search and a retrieval-augmented generation assistant) is a **feature of the Knowledge Infrastructure platform**, not a separate transformation. Its purpose is to make the firm's governed knowledge faster and more naturally accessible than keyword search alone allows.

## 2. Guiding Principles

1. **Governed content only** — the AI assistant retrieves exclusively from content that has passed the platform's classification and lifecycle review process; it does not index ungoverned or unclassified sources
2. **Confidentiality by design, not by exception** — access control is enforced at the retrieval layer itself, so the AI assistant structurally cannot return content across an ethical wall, rather than relying on the assistant to "choose" not to
3. **Grounded, attributable answers** — the assistant must cite the source content it draws from, so consultants can verify and trust its answers rather than treat them as unverifiable output
4. **Human judgment remains primary** — the AI assistant supports a consultant's search for information; it does not replace professional judgment on how that information is applied to client work
5. **Gated release, not fixed-date release** — AI features are released only once they meet defined accuracy and grounding thresholds, even if that means decoupling them from an otherwise-ready platform launch

## 3. The Confidentiality Requirement (Scoped, Not Designed, Here)

The requirement that AI retrieval must respect client-confidentiality and ethical-wall boundaries is treated as a **hard, non-negotiable platform requirement** captured here at the strategy level. The specific technical mechanism for enforcing this (e.g., how access filtering interacts with retrieval indexing) is a Platform Engineering design responsibility, scoped formally in `../07 Decisions/003 AI Confidentiality Safeguard Scope.md`.

## 4. Data Strategy Principles

- Data used to power search and AI retrieval is scoped strictly to firm knowledge content already classified under the taxonomy spine — no client system data, personal data beyond what's contained in existing documents, or external data sources are introduced without a separate governance review
- Data residency and cross-border transfer rules (per region) govern where content and any associated embeddings/indexes may be hosted

## 5. Success Measures

AI success is measured at the delivery level (search success rate, grounding accuracy — see PM Delivery repository) against thresholds set here as non-negotiable release gates, not aspirational targets.
