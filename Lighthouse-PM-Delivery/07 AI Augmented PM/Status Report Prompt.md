# AI-Augmented PM: Status Report Drafting

## Use Case
Turning raw tracker data (budget, schedule, risks) into the narrative sections of a monthly status report, ahead of the Program Steering Committee meeting.

## Prompt Used

```
You are helping a project manager draft the "Summary" and "This Month's
Highlights" sections of a monthly status report for a Steering Committee
audience. Use a neutral, factual tone — no hype, no minimizing of risk.

Here is this month's raw data:
- Budget: €512,000 spent of €750,000 (68%)
- Schedule: Month 13 of 18
- Migration: Wave 1 100% complete, Wave 2 70% complete, Wave 3 not started
- Sprint 4 AI pilot: search success 78% (target 85%), grounding accuracy 89%
  (target 95%) — below target
- Decision made this month: AI assistant launch decoupled from EMEA go-live
  (Decision 003)
- Ethical-wall access control design signed off by Compliance this month

Draft a 3-4 sentence Summary and 3 bullet-point Highlights section.
```

## Example Output (AI Draft)

> **Summary:** The program remains on track for overall scope and end date, with one schedule adjustment approved this month (Decision 003 — phased AI assistant launch). Migration Wave 2 (Americas) is in progress and tracking to plan. Budget shows a contingency draw from Month 5, with reserve remaining.
>
> **Highlights:**
> - Sprint 4 AI assistant pilot completed; results below target triggered Decision 003 (phased launch)
> - Migration Wave 2 (Americas) 70% complete, tracking to Month 11 end date
> - Ethical-wall access control design finalized and approved by Compliance & Data Privacy Office

## What the PM Did With It

Reviewed for tone (confirmed it didn't understate the pilot shortfall), added the specific budget reserve figure the AI had generalized, and used it as the final Summary/Highlights text in `05 Controls/Status Reports/Status Report - Month 13.md`.
