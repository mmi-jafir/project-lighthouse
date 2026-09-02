# Automation: Risk Escalation Trigger

**Introduced:** Month 4 (program setup)
**Owner:** Program Manager

## Trigger
A risk in `02 Planning/RAID Log.xlsx` is marked "High" severity and remains "Open" for more than 14 days without a logged mitigation update.

## Logic
Automated check against the Risk Register's Severity and Status/last-updated fields. Any risk meeting both conditions is flagged for escalation.

## Output
Automated notification to the Program Manager and the risk's Owner, prompting either a mitigation update or formal escalation to the Program Steering Committee via the escalation email template.

## Flowchart

```mermaid
flowchart TD
    A[Check Risk Register: Severity and Last Updated fields] --> B{Severity = High?}
    B -- No --> A
    B -- Yes --> C{Open more than 14 days without update?}
    C -- No --> A
    C -- Yes --> D[Flag for escalation]
    D --> E[Notify Program Manager and Risk Owner]
    E --> F{Mitigation update logged?}
    F -- No --> G[Formal escalation to Steering Committee via Escalation template]
    F -- Yes --> A
```

## Why It Matters
Prevents high-severity risks from silently aging without action — a common failure mode in programs with a large, distributed risk register across multiple regions and workstreams.

## Related
`02 Planning/RAID Log.xlsx`, `06 Communications/Templates/Escalation.md`
