# Decision 002 — Taxonomy Standard vs. Regional Flexibility

**Status:** Decided
**Date:** Month 2 (transformation design phase)
**Decision Owner:** Knowledge Governance Council (recommended) → Transformation Steering Committee (approved)
**Related:** `../04 Technology Strategy/Information Architecture Overview.md`, `001 Federated vs Central Governance.md`

---

## Context

Having adopted a federated governance philosophy (Decision 001), the transformation team needed to decide precisely **where the line sits** between the mandatory global taxonomy spine and permitted regional flexibility — a more granular question than the governance philosophy itself.

## Problem

Define exactly which taxonomy fields must be globally standardized versus which may vary by region, in a way specific enough to guide the information architecture design before migration and platform build work began.

## Options Considered

**A. Minimal global spine** — only "Document Type" standardized globally; nearly everything else regionally defined.
**B. Maximal global spine** — Practice, Industry, Document Type, Confidentiality Classification, and most descriptive fields standardized globally, leaving minimal regional flexibility.
**C. Moderate spine (four core fields)** — Practice, Industry, Document Type, and Confidentiality Classification standardized globally; all other descriptive tagging left to regional extension.

## Analysis

| Option | Cross-Regional Search Quality | Regional Flexibility | Design Complexity |
|---|---|---|---|
| A. Minimal spine | Poor — most useful filtering remains inconsistent across regions | High | Low |
| B. Maximal spine | Excellent | Very low — likely to trigger the same resistance the federated model was designed to avoid | High |
| C. Moderate spine (four fields) | Strong — covers the fields most useful for cross-regional search and AI retrieval | Moderate-high | Moderate |

Option C was selected as the fields most essential to firm-wide search, reuse, and confidentiality enforcement — the transformation's core objectives — while leaving room for regions to add locally meaningful tags without waiting for central approval on every addition.

## Recommendation

Adopt a **four-field mandatory global spine** (Practice, Industry, Document Type, Confidentiality Classification), with all other classification needs addressed through the regional extension layer.

## Decision

Approved by the Transformation Steering Committee in Month 2. This became the specification handed to the delivery team ahead of taxonomy and information architecture design.

## Impact

- Gave the delivery team (see PM Delivery repository) a clear, bounded specification to design against from the start
- When the EMEA/APAC taxonomy conflict arose during delivery, it was resolved within this already-agreed structure rather than reopening the fundamental spine-vs-flexibility question
- Confidentiality Classification's inclusion in the mandatory spine was specifically important, since it is the field the AI/RAG confidentiality safeguard depends on (see `003 AI Confidentiality Safeguard Scope.md`)

## Stakeholders Informed

Transformation Steering Committee (approval), Knowledge Governance Lead (specification owner), Technology Lead (informed for platform design), Regional Governance Contacts (informed of their extension-layer authority).
