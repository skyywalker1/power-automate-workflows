
## Workflow Overview

**Name:** ETQ – Notify Assigned To  
**Platform:** Power Automate  
**Trigger:** When an item is created or modified (SharePoint)

### Business Problem
Items created or updated in the ETQ tracking list were frequently assigned
to users without consistent notification. This led to missed actions,
delayed responses, and reliance on manual follow‑up.

### Solution
This workflow automatically detects when an item is created or updated,
checks whether the **Assigned To** field is populated, and sends an email
notification to the assigned user.

The automation ensures ownership changes are immediately visible
and actionable without manual intervention.

### Data Sources
- SharePoint Online list (ETQ tracking data)
- SharePoint Person field (Assigned To)
