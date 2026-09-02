# Decision 003 — AI Confidentiality Safeguard Scope

**Status:** Decided
**Date:** Month 3 (transformation design phase, ahead of delivery Sprint 0)
**Decision Owner:** Transformation Steering Committee, with Compliance & Data Privacy Office as advisor
**Related:** `../04 Technology Strategy/AI And Data Strategy.md`, `Lighthouse-PM-Delivery/02 Planning/RAID Log.xlsx` (R002)

---

## Context

The AI/Data Strategy establishes that AI retrieval must never surface client-confidential content across an ethical wall. Before delivery began designing the AI/RAG capability, the Steering Committee needed to decide **how much of this safeguard to specify at the program level** versus leave to Platform Engineering's technical design — a scope boundary question, not a technical design question.

## Problem

Decide whether the transformation program should specify the AI confidentiality safeguard only as a business requirement, or attempt to prescribe the specific technical mechanism (e.g., retrieval-time filtering vs. separate per-engagement indexes) at the program level.

## Options Considered

**A. Prescribe the technical mechanism** — the program specifies exactly how confidentiality-aware retrieval must be technically implemented.
**B. Specify only the business requirement** — the program states the non-negotiable outcome (zero cross-wall exposure) and defined evaluation criteria, leaving the technical mechanism entirely to Platform Engineering.
**C. Specify the requirement plus mandatory validation criteria** — state the business requirement, plus require that any proposed technical approach be validated against a defined test suite before AI release, without prescribing the mechanism itself.

## Analysis

| Option | Speed to Design | Risk of Wrong-Altitude Program Involvement | Assurance of Actually Meeting the Requirement |
|---|---|---|---|
| A. Prescribe mechanism | Slower — program lacks the technical expertise to do this well | High — risks the program making a poor technical choice it isn't qualified to make | Uncertain — a prescribed mechanism might not fit the eventual platform architecture |
| B. Business requirement only | Fast | Low | Lower — no explicit check that the requirement was actually met before release |
| C. Requirement + validation criteria | Fast | Low | High — technical freedom for Platform Engineering, combined with an explicit gate |

## Recommendation

Adopt **Option C**: the transformation program specifies the requirement (zero cross-wall exposure) and mandates a pre-release validation test (access control testing against defined ethical-wall scenarios), while leaving the specific technical retrieval design entirely to Platform Engineering.

## Decision

Approved by the Transformation Steering Committee in Month 3. This decision directly shaped the Quality Management Plan's AI Pilot Gate at the delivery level, and the confidentiality access control testing item in the Go-Live Checklist.

## Impact

- Kept the transformation program's involvement at the correct altitude — setting requirements and gates, not designing technical mechanisms it isn't positioned to design well
- Gave the delivery team clear release criteria (documented as R002 in the RAID Log) without constraining their technical approach
- The validation gate was exercised in practice during delivery, when confidentiality access control testing was required before the EMEA go-live (see `Lighthouse-PM-Delivery/03 Delivery/Launch/Go Live Checklist.xlsx`)

## Stakeholders Informed

Transformation Steering Committee (approval), Compliance & Data Privacy Office (validation criteria co-design), Technology Lead (informed of the requirement and gate, free to design the mechanism).
