# Migration Strategy
### Knowledge Infrastructure Workstream — Project Lighthouse

**Version:** 1.1 (updated post–Decision 001)
**Related:** `Migration Wave Plan.xlsx`, `09 Decisions/001 Budget Change Due to Migration Complexity.md`

---

## 1. Approach

Migration proceeds in three regional waves rather than a single global cutover, to manage complexity, spread governance and change-management effort, and allow lessons from earlier waves to improve later ones.

```text
Keep → Clean → Migrate → Archive → Delete
```

Each content source is assessed against this lifecycle before migration, per the original knowledge audit.

## 2. Migration Waves

| Wave | Region | Timing | Content Volume (est.) |
|---|---|---|---:|
| Wave 1 | EMEA | Months 5–8 | ~4,800 documents |
| Wave 2 | Americas | Months 8–11 | ~5,600 documents |
| Wave 3 | APAC | Months 11–13 | ~3,900 documents |

## 3. Revised Approach Post–Decision 001

Following the Wave 1 audit, legacy metadata quality was found to be significantly lower than originally estimated, increasing manual classification effort. An automated metadata-cleanup utility (duplicate detection, missing-owner flagging, stale-content flagging) was introduced ahead of Waves 2 and 3 to reduce manual effort, funded via a partial contingency draw (see Decision 001).

## 4. Classification Rules

Content is classified against the taxonomy spine (Practice, Industry, Document Type, Confidentiality Classification) defined under the federated taxonomy model (see `09 Decisions/002 Taxonomy Governance Approach.md`), plus optional regional extension tags.

## 5. Confidentiality Handling During Migration

Content flagged as client-confidential during audit is migrated with access restricted to the original engagement team by default, pending formal ethical-wall configuration in the platform's access model. No confidential content is exposed to broader search indexing until this configuration is verified.

## 6. Cutover Approach

Each regional wave uses a phased cutover: legacy source remains read-only accessible for 30 days post-migration as a fallback, then is archived. No wave proceeds to cutover until the prior wave's lessons have been incorporated.
