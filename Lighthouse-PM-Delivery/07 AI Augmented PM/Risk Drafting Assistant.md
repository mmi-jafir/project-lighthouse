# AI-Augmented PM: Risk Register Drafting

## Use Case
Turning a brief, informally described concern into a properly structured RAID Log entry.

## Prompt Used

```
Turn this rough concern into a structured risk register entry with:
Risk Description, Category, Likelihood, Impact, Severity, Owner,
Mitigation. Use our standard categories: Delivery, Compliance, Adoption,
Regulatory, Resourcing, Vendor.

Rough concern: "I'm a bit worried that if the AI assistant ever mixes up
content between two clients that are actually competitors, that would be
really bad — like, firm-reputation bad, not just an annoying bug."
```

## Example Output (AI Draft)

| Field | Value |
|---|---|
| Risk Description | AI/RAG assistant surfaces client-confidential content across an ethical wall (e.g., between competing client engagements) |
| Category | Compliance |
| Likelihood | Medium |
| Impact | High |
| Severity | High |
| Owner | Technology Lead |
| Mitigation | Confidentiality-aware access design scoped as a hard requirement prior to AI rollout |

## What the PM Did With It

Used this directly as R002 in `02 Planning/RAID Log.xlsx`, adjusting only the Owner field after confirming responsibility sat with the Technology Lead rather than the original reporter (a Practice Area Leader who raised the concern informally).
