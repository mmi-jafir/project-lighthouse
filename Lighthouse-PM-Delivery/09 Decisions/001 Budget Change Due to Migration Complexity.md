# Decision 001 — Budget Change Due to Migration Complexity

**Status:** Decided
**Date:** Month 5
**Decision Owner:** Program Manager (recommended) → Program Steering Committee (approved)
**Related:** `02 Planning/RAID Log.xlsx` (R001, I001), `02 Planning/Budget.xlsx`, `05 Controls/Budget vs Actual.xlsx`

---

## Context

Following the Wave 1 (EMEA) migration audit, the Migration Lead identified that legacy content across regional SharePoint sites and shared drives carried significantly more inconsistent, missing, or conflicting metadata than the original knowledge audit estimated. Manual classification effort required to bring this content up to the platform's taxonomy standard is approximately 30% higher than planned for the remaining migration waves (Americas, APAC).

## Problem

The approved migration budget (€120,000) is insufficient to complete Waves 2 and 3 at the required quality bar without either additional funding, reduced scope, or a schedule extension.

## Options Considered

**A. Increase budget** — draw down the €30,000 contingency reserve to cover the shortfall.
**B. Reduce scope** — migrate only the highest-priority content (e.g., top 60% by usage) and archive or exclude the remainder.
**C. Extend timeline** — push the migration completion date back by 4–6 weeks to allow more manual cleanup time within the existing budget.
**D. Increase automation** — invest a smaller amount in an automated metadata-cleanup script to reduce manual effort, partially offsetting the shortfall.

## Analysis

| Option | Cost Impact | Schedule Impact | Quality Impact | Risk |
|---|---|---|---|---|
| A. Increase budget | Uses full contingency reserve | None | Maintains full scope and quality | Leaves no reserve for later risks |
| B. Reduce scope | None | None | Excludes some lower-priority but still valuable content | Risk of excluding content later requested by consultants |
| C. Extend timeline | None | Delays global rollout by 4–6 weeks | Maintains quality | Delays realization of productivity benefits |
| D. Increase automation | Moderate (~€15,000 from contingency) | Minimal | Maintains most quality with faster throughput | Automation script may not fully replace manual judgment on ambiguous content |

A combination of **A (partial) and D** was assessed as the strongest path: automating the most mechanical parts of metadata cleanup (duplicate detection, missing-owner flagging) reduces the manual burden meaningfully, while a partial contingency draw covers the remaining gap without fully depleting the reserve or delaying the program.

## Recommendation

Approve a **€15,000 contingency draw** to fund an automated metadata-cleanup utility for Waves 2 and 3, combined with a **retained €15,000 contingency reserve** for remaining program risks. No scope reduction and no schedule extension.

## Decision

Approved by the Program Steering Committee in Month 5. Contingency budget reallocated: €15,000 to Migration (automation tooling), €15,000 retained as reserve.

## Impact

- `02 Planning/Budget.xlsx` Contingency line reduced from €30,000 available to €15,000 remaining reserve
- Migration approach for Waves 2–3 updated to include an automated pre-classification pass before manual review
- No change to overall program timeline or scope

## Stakeholders Informed

Program Steering Committee (approval), Migration Lead (implementation), Regional Leads — Americas and APAC (informed of revised migration approach ahead of their waves).
