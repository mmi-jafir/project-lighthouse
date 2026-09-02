# Product Backlog
### Knowledge Search & AI Assistant Workstream — Project Lighthouse

**Delivery Approach:** Agile (within a hybrid program governance structure — see `Lighthouse-Transformation-Strategy/02 Operating Model/`)
**Product Owner:** Technology Lead
**Related:** `Sprint Reports/`, `09 Decisions/003 Launch Date Adjustment.md`

---

## Epics

1. **Foundational Search** — basic keyword search across migrated content
2. **Metadata & Filtering** — filter search results by taxonomy, region, practice
3. **Semantic Search** — meaning-based retrieval beyond exact keyword match
4. **AI Assistant (RAG)** — conversational assistant grounded in firm knowledge
5. **Confidentiality-Aware Retrieval** — ensures AI never surfaces content across an ethical wall

## Sprint Plan Summary

| Sprint | Goal | Key Backlog Items | Outcome |
|---|---|---|---|
| Sprint 0 — Discovery | Define MVP and success metrics | User interviews, search pain-point analysis, technical discovery | Complete — see `Sprint Reports/Sprint 0 Discovery Report.md` |
| Sprint 1 | Build basic keyword search | Index migrated Wave 1 content; basic query UI | Complete |
| Sprint 2 | Add filters and metadata | Filter by taxonomy spine fields (practice, industry, doc type) | Complete |
| Sprint 3 | Add semantic search | Embed content; implement vector similarity search | Complete |
| Sprint 4 | Pilot with 50 users | Deploy to pilot group; collect usage and accuracy data | Complete — below target, see `Sprint Reports/Sprint 4 Pilot Report.md` and `09 Decisions/003` |
| Sprint 5 | Improve based on feedback | Tune retrieval ranking; expand indexed content; fix grounding gaps | Complete |
| Sprint 6 | Add AI/RAG assistant functionality | Conversational interface; confidentiality-aware retrieval guardrails | Complete |

## Current Backlog (Post-Sprint 6)

| ID | Item | Priority | Status |
|---|---|---|---|
| B-101 | Expand AI assistant to Americas content index | High | In Progress |
| B-102 | Add citation/source display to AI assistant answers | High | In Progress |
| B-103 | Extend confidentiality-aware retrieval to regional extension taxonomy tags | High | In Progress |
| B-104 | Improve grounding accuracy for APAC-language content | Medium | Backlog |
| B-105 | Add "was this helpful" feedback capture in AI assistant UI | Medium | Backlog |
| B-106 | Expert-finder integration — surface a human SME alongside AI answers | Low | Backlog |

## Definition of Done

- Feature deployed to the relevant environment
- Confidentiality-aware access rules verified for the feature (no cross-engagement content leakage)
- Success metric (search success rate or grounding accuracy) measured against target
- Documented in the relevant Sprint Report
