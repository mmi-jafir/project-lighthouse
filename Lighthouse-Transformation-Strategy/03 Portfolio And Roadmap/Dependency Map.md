# Dependency Map
### Project Lighthouse — Knowledge Infrastructure Transformation

**Version:** 1.0
**Related:** `Transformation Roadmap.md`

---

## 1. Cross-Workstream Dependencies

```text
Governance & Taxonomy Design
        │
        ├──► Migration (classification rules must exist before content can be migrated)
        │
        └──► Technology / Platform (taxonomy structure shapes search indexing design)
                    │
                    ├──► AI / RAG (retrieval quality depends on governed, classified content)
                    │
                    └──► Regional Rollout (platform must be stable before go-live)

Change & Adoption Management
        │
        └──► Regional Rollout (training and incentive alignment must precede go-live)

Compliance & Confidentiality Design
        │
        ├──► Migration (confidential content handling rules needed before migration)
        └──► AI / RAG (ethical-wall access design is a hard prerequisite for AI release)
```

## 2. Critical Path Dependencies

| Dependency | Risk if Delayed |
|---|---|
| Taxonomy spine finalized before migration begins | Migration would need to be redone or content would be inconsistently classified |
| Ethical-wall access design approved before AI assistant release | Confidentiality breach risk — treated as a hard release gate, not a soft target |
| Regional governance contacts onboarded before regional rollout | Local adoption and ongoing content quality would lack an accountable owner |

## 3. Cross-Reference to Delivery-Level Dependencies

Task-level dependencies within the delivery project itself (e.g., Wave 2 migration depending on Wave 1 lessons) are tracked in `Lighthouse-PM-Delivery/02 Planning/RAID Log.xlsx` (Dependencies sheet). This document captures dependencies at the program/workstream level, one altitude above that detail.
