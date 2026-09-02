# Scope Statement
### Knowledge Infrastructure Workstream — Project Lighthouse

**Version:** 1.0
**Status:** Approved
**Related Document:** `Project Charter.md`

---

## 1. Project Scope Description

This project delivers a governed, searchable, AI-enabled Knowledge Infrastructure platform for Solstice Advisory's global consultant base. It replaces fragmented content sources with a unified, classified, and access-controlled knowledge environment, supported by semantic search and an AI-assisted retrieval layer, and underpinned by a sustainable governance model.

## 2. Deliverables

| Deliverable | Description |
|---|---|
| Knowledge Audit | Inventory and quality assessment of existing content sources by office/region |
| Information Architecture | Taxonomy (practice × industry × geography), metadata schema, content classification model |
| Migration | Migrated, cleaned, and classified content, delivered in regional waves |
| Platform | Configured knowledge platform with search and access control |
| AI/RAG Layer | AI-assisted retrieval scoped to respect confidentiality and ethical-wall requirements |
| Governance Model | Roles, review process, content lifecycle, and federated global/regional governance structure |
| Change & Adoption Plan | Training, communications, and incentive alignment to drive usage |
| Automation | Automated alerts and reporting to support ongoing platform operations |

## 3. Scope Boundaries

### In Scope

- Audit and classification of content from SharePoint, Confluence, shared drives, and select email archives
- Design and implementation of a firm-wide taxonomy spanning practice, industry, and geography
- Migration of prioritized content in regional waves
- Implementation of unified search and an AI/RAG assistant layer
- Design of confidentiality-aware access controls (ethical walls) as a platform requirement
- Governance model design, including federated global/regional ownership
- Training, communications, and adoption support across consultant grades
- Automation of routine platform operations (stale content alerts, status reporting)

### Out of Scope

- Replacement of client-delivery tools (e.g., engagement management systems) unrelated to knowledge content
- Firm-wide IT infrastructure modernization beyond what is required for the platform
- Compensation, staffing, or promotion model redesign (addressed only as a recommendation within the adoption strategy)
- Detailed technical design of the AI/RAG retrieval architecture — this project scopes the *requirement* (confidentiality-aware retrieval) and hands detailed technical design to the platform engineering function

## 4. Acceptance Criteria

- Migrated content reaches 90%+ of the prioritized inventory, correctly classified
- Search success rate reaches 85%, verified through user testing
- AI-answer grounding accuracy reaches 95%, verified through evaluation sampling
- Governance roles are assigned and active for 95%+ of published content
- No confirmed ethical-wall or confidentiality breach during pilot or rollout

## 5. Assumptions

- Regional offices will provide content owners and reviewers to support classification
- The firm's existing identity and access management system can be extended to support the platform's access model

## 6. Constraints

- Client-confidentiality and cross-border data regulations govern access and hosting design
- Migration must proceed without disrupting active client engagements
- Budget is fixed at €750,000; scope trade-offs are managed through the change control process (see `09 Decisions/`)

## 7. Change Control

Any request to modify scope, budget, or timeline is logged in `05 Controls/Change Request Log.xlsx` and assessed for impact before approval by the Program Steering Committee.
