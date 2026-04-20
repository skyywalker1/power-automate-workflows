## Flow Logic

This workflow uses an event-driven design to automate notifications
based on changes in SharePoint data.

### Trigger
- The workflow is triggered when an item is **created or modified**
  in the SharePoint ETQ tracking list.

### Compose Action
- A compose step is used to capture or prepare values needed for
  conditional evaluation.
- This helps simplify downstream logic and improves flow readability.

### Condition Check
- The workflow evaluates whether the **Assigned To** field is populated.
- This prevents unnecessary actions when no owner has been assigned.

**Logic outcome:**
- If **Assigned To is blank** → no action is taken.
- If **Assigned To is populated** → notification logic is executed.

### Apply to Each Loop
- SharePoint Person fields return values as an array.
- An **Apply to each** loop is used to safely process one or more
  assigned users.
- This ensures the workflow handles both single and multi-user
  assignments correctly.

### Notification Action
