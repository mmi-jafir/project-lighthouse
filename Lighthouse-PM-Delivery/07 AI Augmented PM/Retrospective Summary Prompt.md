# AI-Augmented PM: Retrospective Synthesis

## Use Case
Synthesizing scattered input from a Sprint 4 retrospective (collected via sticky notes / chat comments) into a coherent summary for the Sprint 5 planning session.

## Prompt Used

```
Synthesize this retrospective input into three sections: What Went Well,
What Didn't, and What We'll Change. Group similar comments together
rather than listing every comment individually.

Raw input:
- "pilot users actually liked using it, positive feedback overall"
- "grounding accuracy was rough for older documents"
- "some doc types weren't well represented in embeddings"
- "process for flagging outdated docs is too manual, we should automate more"
- "50 users was a good pilot size, not too chaotic"
- "took too long to notice which category of documents was causing the
  low accuracy — should have sliced the data earlier"
```

## Example Output (AI Draft)

> **What Went Well:** Pilot user feedback was positive overall, and the 50-user pilot size struck a good balance — large enough to be meaningful, small enough to manage closely.
>
> **What Didn't:** Grounding accuracy was weaker for older and less-represented document types, and the team took longer than ideal to isolate which content category was driving the shortfall.
>
> **What We'll Change:** Slice evaluation data earlier by document type/age to catch this pattern faster next time, and reduce reliance on manual flagging of outdated content by expanding automation.

## What the PM Did With It

Used this synthesis directly as the basis for the "Follow-Up Actions" section in `03 Delivery/Agile/Sprint Reports/Sprint 4 Pilot Report.md`, and flagged the "slice data earlier" lesson as a standing practice for future sprint evaluations.
