# Decision 002 — Taxonomy Governance Approach

**Status:** Decided
**Date:** Month 3
**Decision Owner:** Knowledge Governance Lead (recommended) → Program Steering Committee (approved)
**Related:** `02 Planning/RAID Log.xlsx` (I002), Transformation Strategy repo — `Lighthouse-Transformation-Strategy/02 Operating Model/Federated vs Central Governance.md`

---

## Context

During information architecture design, EMEA and APAC regional offices raised conflicting preferences for how content should be classified. EMEA requested taxonomy categories aligned closely to European regulatory and industry structures, while APAC requested categories reflecting locally distinct service lines not used elsewhere in the firm. A single, rigid global taxonomy risked poor adoption in one or both regions; fully independent regional taxonomies risked breaking global search and cross-region knowledge reuse — the core value proposition of the program.

## Problem

Decide whether the platform should use one fixed global taxonomy, fully independent regional taxonomies, or a structure that accommodates both global consistency and regional relevance.

## Options Considered

**A. Single global taxonomy** — one fixed classification structure applied identically worldwide.
**B. Fully independent regional taxonomies** — each region defines and manages its own structure.
**C. Federated taxonomy** — a global "spine" (practice, industry, document type) mandatory everywhere, with an optional regional extension layer for locally relevant categories.

## Analysis

| Option | Global Searchability | Regional Relevance | Governance Complexity | Adoption Risk |
|---|---|---|---|---|
| A. Single global taxonomy | High | Low | Low | High — regional offices may resist or work around it |
| B. Independent regional taxonomies | Low | High | High — no consistent global standard | Low locally, but undermines global reuse goal |
| C. Federated taxonomy | High (via mandatory spine) | High (via regional extension) | Medium | Low — balances both needs |

Option C directly supports the federated global/regional governance model already adopted at the program level (see the Transformation Strategy repository), making it the most consistent choice architecturally as well as practically.

## Recommendation

Adopt the **federated taxonomy model (Option C)**: a mandatory global spine (Practice, Industry, Document Type, Confidentiality Classification) applied to all content firm-wide, with a regional extension layer that regions may populate with locally relevant tags, reviewed centrally for overlap and consistency.

## Decision

Approved by the Program Steering Committee in Month 3. Knowledge Governance Lead to publish the global spine standard and regional extension guidelines before Wave 1 migration begins.

## Impact

- Information architecture design updated to formally separate mandatory spine fields from optional regional extension fields
- Regional Knowledge Contacts given authority to propose and manage extension tags within their region, subject to periodic central review
- Slight increase in governance review effort to prevent regional tag sprawl, offset by improved regional adoption

## Stakeholders Informed

Program Steering Committee (approval), Regional Leads — EMEA and APAC (direct resolution of their request), Practice Area Leaders (informed of global spine structure), Technology Lead (search indexing updated to support both spine and extension fields).
