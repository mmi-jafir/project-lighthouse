# Decision 003 — Launch Date Adjustment for EMEA Go-Live

**Status:** Decided
**Date:** Month 13
**Decision Owner:** Program Manager (recommended) → Program Steering Committee (approved)
**Related:** `02 Planning/Schedule And WBS.xlsx`, `02 Planning/RAID Log.xlsx` (R007), `03 Delivery/Launch/Launch Plan.md`

---

## Context

The AI Search Pilot (Sprint 4, 50 users) completed in Month 12 with search success at 78% against an 85% target, and AI-answer grounding accuracy at 89% against a 95% target. While within an acceptable range for a pilot, both metrics fell short of the threshold set for proceeding directly to regional go-live as originally scheduled in Month 14.

## Problem

Decide whether to proceed with the EMEA regional go-live as scheduled in Month 14, despite the AI layer not yet meeting target performance, or to adjust the launch timeline.

## Options Considered

**A. Proceed as scheduled** — launch in Month 14 with the AI assistant clearly labeled as "in beta," continuing improvement post-launch.
**B. Delay go-live** — extend the pilot and iteration phase by 4 weeks to bring AI performance closer to target before regional rollout.
**C. Phased feature launch** — launch core search and platform functionality on schedule in Month 14, but hold back the AI assistant specifically until it meets target, releasing it as a follow-on feature.

## Analysis

| Option | Schedule Impact | User Experience Risk | Benefit Realization | Risk |
|---|---|---|---|---|
| A. Proceed as scheduled | None | Risk of poor first impressions with an underperforming AI feature | Full benefit case (incl. AI) starts immediately, at reduced quality | High — a weak first experience with the flagship AI feature could damage adoption momentum firm-wide |
| B. Delay go-live | Delays core platform benefits (search, migration) by 4 weeks | Avoided | Delayed 4 weeks | Moderate — un-related core benefits are delayed unnecessarily |
| C. Phased feature launch | None for core platform; AI assistant delayed ~3–4 weeks | Minimized — users get a solid core experience first | Core benefits realized on schedule; AI benefit delayed slightly | Low — decouples a stable, ready deliverable from one still being tuned |

## Recommendation

Adopt **Option C — phased feature launch**. Launch core platform and search functionality in EMEA on the original Month 14 schedule. Hold the AI assistant in continued iteration and release it as a follow-on feature once it reaches the 85% search success / 95% grounding accuracy thresholds, expected within approximately 3–4 additional weeks.

## Decision

Approved by the Program Steering Committee in Month 13. EMEA go-live proceeds on schedule for core platform functionality; AI assistant release decoupled and re-targeted for early Month 15, pending threshold achievement.

## Impact

- `02 Planning/Schedule And WBS.xlsx` updated to reflect the AI assistant as a distinct, trailing release milestone within the EMEA rollout wave
- Launch communications revised to clearly frame the AI assistant as "coming soon" rather than day-one functionality, managing user expectations
- No change to overall program end date; contingency schedule buffer in the Rollout phase absorbs the AI assistant's short delay

## Stakeholders Informed

Program Steering Committee (approval), Regional Lead — EMEA (updated go-live scope), Consultants/end users (updated via launch communications), Technology Lead (continued AI iteration plan).
