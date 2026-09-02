# Automation
### Knowledge Infrastructure Workstream — Project Lighthouse

This folder documents PM process automations used to run the project itself more efficiently — distinct from the platform's own AI features (documented in the Transformation Strategy repository) and from AI-assisted drafting (documented in `../07 AI Augmented PM/`).

Each automation below follows the same format: trigger → logic → output → owner.

| Automation | Purpose |
|---|---|
| `Stale Content Alerts.md` | Flags migrated content that hasn't been reviewed within its lifecycle window |
| `Risk Escalation Trigger.md` | Automatically escalates high-severity risks that remain open past a threshold |
| `Overdue Task Notification.md` | Notifies task owners and the Project Manager of overdue WBS items |
| `Status Report Auto Generation.md` | Assembles a draft status report from live tracker data ahead of steering meetings |
| `Change Request Routing.md` | Routes new change requests to the correct approver based on impact size |
| `Meeting Action Tracking.md` | Extracts action items from meeting notes into the tracker automatically |

These were introduced incrementally over the course of the project as recurring manual effort was identified — several were prompted directly by friction observed during Migration Wave 1 and the Sprint 4 pilot.
