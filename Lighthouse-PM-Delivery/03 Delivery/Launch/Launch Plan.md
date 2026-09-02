# Launch Plan
### Knowledge Infrastructure Workstream — Project Lighthouse

**Version:** 1.1 (updated post–Decision 003)
**Related:** `Go Live Checklist.xlsx`, `09 Decisions/003 Launch Date Adjustment.md`, `06 Communications/Employees/`

---

## 1. Launch Approach

Launch proceeds regionally, in the same sequence as the migration waves, so each region goes live on a platform already populated with its own migrated and classified content.

| Region | Planned Go-Live | Scope at Go-Live |
|---|---|---|
| EMEA | Month 14 | Core platform, search, filtering (AI assistant follows ~Month 15 per Decision 003) |
| Americas | Month 15 | Core platform, search, filtering, AI assistant (if thresholds met by this point) |
| APAC | Month 16–17 | Full platform including AI assistant |

## 2. Phased Feature Release (Per Decision 003)

The AI assistant is launched as a **trailing feature** in EMEA rather than a day-one capability, following pilot results that fell short of the grounding-accuracy and search-success thresholds. This avoids a poor first impression with the program's most visible feature while allowing the stable core platform (search, filtering, migrated content) to deliver value immediately.

## 3. Pre-Launch Checklist Categories

See `Go Live Checklist.xlsx` for the full checklist. Categories:
- Content readiness (migration complete, classification audit passed)
- Platform readiness (performance testing, access control verification)
- Confidentiality readiness (ethical-wall access testing signed off by Compliance)
- Change readiness (training delivered, communications sent, support channel live)
- Governance readiness (regional Knowledge Governance contacts active)

## 4. Go-Live Day Activities

1. Final access control verification
2. Legacy source systems set to read-only (30-day fallback window begins)
3. Go-live announcement communication sent to the regional consultant population
4. Support channel and FAQ published
5. Go-live confirmed by Regional Lead and Program Manager

## 5. Post-Launch Support

- **Hypercare period:** 2 weeks of elevated support responsiveness per region following go-live
- **Feedback loop:** in-platform feedback widget monitored daily during hypercare
- **Escalation:** issues affecting confidentiality or data integrity escalated immediately to the Program Manager and Compliance & Data Privacy Office, regardless of hypercare status

## 6. Rollback Plan

If a critical issue is identified within the first 5 business days of a regional go-live (e.g., a confidentiality control failure), the region reverts to legacy read-only sources while the issue is resolved, per the 30-day fallback window.
