# Information Architecture Overview
### Project Lighthouse — Knowledge Infrastructure Transformation

**Version:** 1.0
**Related:** `../07 Decisions/002 Taxonomy Standard vs Regional Flexibility.md`, `Lighthouse-PM-Delivery/09 Decisions/002 Taxonomy Governance Approach.md`

---

## 1. Purpose

Establishes the firm-wide approach to classifying knowledge content — the foundation that both search and AI retrieval quality depend on, per the Digital Maturity Assessment's finding that governance, not technology, was the primary gap.

## 2. Taxonomy Structure (Federated Spine + Extensions)

```text
Global Spine (Mandatory)
├── Practice (e.g., Strategy, Digital, Operations)
├── Industry (e.g., Financial Services, Healthcare, Energy)
├── Document Type (e.g., Case Study, Methodology, Proposal, Framework)
└── Confidentiality Classification (Client-Confidential / Firm IP / Credentials / Thought Leadership)

Regional Extension (Optional, Region-Owned)
└── Locally relevant tags (e.g., regional service lines, local regulatory categories)
```

## 3. Content Classification Tiers

| Tier | Definition | Reuse Rule |
|---|---|---|
| Client-Confidential | Deliverables and work product tied to a specific client engagement | Restricted to the original engagement team by default; not searchable firm-wide without explicit reclassification |
| Firm IP | Frameworks, methodologies, tools, and accelerators owned by the firm | Broadly reusable across engagements, subject to attribution/version control |
| Credentials | Client-approved, sanitized case summaries for external use | Reusable in proposals and business development |
| Thought Leadership | Market and sector point-of-view content | Broadly reusable and externally shareable |

## 4. Metadata Standard

Every document carries: Owner, Practice, Industry, Document Type, Confidentiality Classification, Effective Date, Review Date, and Version — the minimum fields required for both governance accountability and AI retrieval quality.

## 5. Relationship to the Federated Governance Decision

This architecture directly implements the federated governance principle established in `../02 Operating Model/Federated vs Central Governance.md`, and formalizes the same resolution reached operationally in `Lighthouse-PM-Delivery/09 Decisions/002 Taxonomy Governance Approach.md`.

## 6. Scope Boundary

This document defines the *classification model*. It does not define the underlying database schema, search indexing implementation, or embedding strategy for AI retrieval — those are Platform Engineering design decisions built on top of this architecture.
