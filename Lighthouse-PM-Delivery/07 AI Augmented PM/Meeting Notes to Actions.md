# AI-Augmented PM: Meeting Notes → Action Items

## Use Case
Converting raw, informally captured meeting notes into structured action items for the shared tracker (feeds `04 Automation/Meeting Action Tracking.md`).

## Prompt Used

```
Extract action items from these raw meeting notes. For each, identify:
Action, Owner, and a reasonable Due Date if mentioned or implied. Output
as a markdown table.

Raw notes:
"Talked about Wave 2 progress, going fine. Sarah mentioned she still
needs to finalize the support channel content before go-live next month
— said she'd have it by end of next week. Also James from APAC confirmed
he's onboarded as the regional contact, that's done already. We agreed
someone needs to double check the training sessions actually got
delivered in EMEA before we tick that box on the go-live checklist —
put that on me I guess, by Friday."
```

## Example Output (AI Draft)

| Action | Owner | Due Date |
|---|---|---|
| Finalize EMEA support channel content | Sarah (Change Lead) | End of next week |
| Confirm Wave 3 regional contact onboarding | James (Regional Lead, APAC) | Complete |
| Verify EMEA training sessions were delivered | Project Manager | Friday |

## What the PM Did With It

Corrected "James" and "Sarah" to their role titles for the formal tracker (per the project's convention of using roles rather than first names in shared documents), and added the item to `05 Controls/Status Reports/` cross-reference for the next update.
