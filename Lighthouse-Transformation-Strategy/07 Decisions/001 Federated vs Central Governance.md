# Decision 001 — Federated vs. Central Governance

**Status:** Decided
**Date:** Month 2 (pre-delivery, during transformation design)
**Decision Owner:** Executive Sponsor (recommended by Transformation Steering Committee)
**Related:** `../02 Operating Model/Federated vs Central Governance.md`, `../02 Operating Model/Target Operating Model.md`

---

## Context

Solstice Advisory's regions (EMEA, Americas, APAC) have historically operated with significant local autonomy over how they organize and share knowledge, reflecting differences in regulatory environment, industry mix, and established local practice. Designing the Knowledge Infrastructure program's governance model required resolving, upfront, how much of that autonomy would be preserved versus standardized before any delivery work began.

## Problem

Decide the fundamental governance philosophy for the program: fully centralized control, fully regional autonomy, or a hybrid — before taxonomy design, platform architecture, or delivery planning could proceed, since this choice shapes all of them.

## Options Considered

**A. Fully central governance** — one global standard for taxonomy, classification, and process, set and enforced centrally.
**B. Fully regional governance** — each region defines its own knowledge management approach independently.
**C. Federated governance** — a mandatory global standard for elements requiring cross-regional consistency (taxonomy spine, confidentiality classification), with defined regional autonomy for elements benefiting from local relevance.

## Analysis

| Option | Cross-Regional Search & Reuse | Regional Buy-In | Implementation Complexity | Long-Term Sustainability |
|---|---|---|---|---|
| A. Fully central | High | Low — risk of being seen as headquarters imposition | Low | Low — historically, centrally-imposed standards at the firm have seen weak regional compliance |
| B. Fully regional | Low — undermines the transformation's core value proposition | High | Low | Low — recreates the fragmentation the program exists to solve |
| C. Federated | High (via mandatory spine) | High (via regional extension autonomy) | Medium | High — balances consistency with buy-in |

Option C was assessed as the only option consistent with the transformation's core objective (firm-wide reuse) while remaining realistic about the firm's actual organizational culture and history.

## Recommendation

Adopt the **federated governance model**: global mandatory standards for taxonomy spine, confidentiality classification, and content lifecycle policy; regional/practice autonomy for extension tags, local adoption approaches, and content stewardship staffing.

## Decision

Approved by the Executive Sponsor in Month 2, early in the Discovery phase and before taxonomy or platform design decisions were finalized. This decision became the foundational operating principle for the entire program and directly shaped the Target Operating Model.

## Impact

- Information architecture design (delivered at the project level) was scoped from the outset to include a regional extension layer, avoiding costly rework
- When EMEA and APAC raised a taxonomy conflict during delivery (Month 3), the resolution was straightforward because the federated principle was already established — see `Lighthouse-PM-Delivery/09 Decisions/002 Taxonomy Governance Approach.md`
- Regional Managing Partners were engaged early as co-owners of the governance model rather than recipients of a centrally imposed standard

## Stakeholders Informed

Transformation Steering Committee (approval), Regional Managing Partners (co-design), Knowledge Governance Lead (implementation), Program Manager (delivery planning basis).
