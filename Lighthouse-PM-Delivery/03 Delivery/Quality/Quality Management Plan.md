# Quality Management Plan
### Knowledge Infrastructure Workstream — Project Lighthouse

**Version:** 1.0
**Related:** `03 Delivery/Agile/`, `03 Delivery/Migration/`, `10 Closure/Benefits Realization.xlsx`

---

## 1. Quality Objectives

| Area | Quality Standard | Measure |
|---|---|---|
| Content Migration | Content correctly classified per taxonomy spine | 90%+ of migrated content passes classification audit |
| Search | Search returns relevant results | Search success rate ≥ 85% (user-tested) |
| AI Assistant | Answers are grounded in accurate, current content | Grounding accuracy ≥ 95% (evaluation sampling) |
| Governance | Content has an accountable owner | 95%+ of published content has an assigned owner |
| Confidentiality | No cross-engagement content exposure | Zero confirmed ethical-wall breaches |

## 2. Quality Assurance Activities

| Activity | Frequency | Owner |
|---|---|---|
| Migration classification audit (sample-based) | Per wave | Knowledge Governance Lead |
| Search success testing with real user tasks | Per sprint (Sprints 1–6) | Technology Lead |
| AI grounding accuracy evaluation (sampled Q&A) | Per sprint (Sprints 4–6) | Technology Lead |
| Confidentiality access control testing | Before each pilot and go-live | Compliance & Data Privacy Office |
| Stale/duplicate content review | Monthly (post-launch, via automation) | Knowledge Governance Lead |

## 3. Quality Control Gates

- **Migration Wave Gate:** a wave is not marked complete until the classification audit passes threshold
- **Pilot Gate:** the AI assistant does not proceed to regional release until it meets grounding accuracy and search success thresholds (see `09 Decisions/003 Launch Date Adjustment.md` for the precedent where this gate was enforced)
- **Go-Live Gate:** confidentiality access control testing must show zero critical findings before any regional go-live

## 4. Issue Escalation

Quality issues identified during QA activities are logged in `02 Planning/RAID Log.xlsx` (Issues sheet) and assessed for whether they block a quality gate. Blocking issues are escalated to the Program Steering Committee if resolution requires a scope, schedule, or budget trade-off (see `09 Decisions/`).

## 5. Continuous Improvement

Each sprint retrospective and each migration wave retrospective feeds lessons into the approach for the next sprint or wave — e.g., the automated metadata-cleanup utility introduced after Wave 1 (Decision 001) and the embedding model retuning after the Sprint 4 pilot.
