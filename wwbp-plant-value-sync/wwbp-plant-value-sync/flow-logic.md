## Flow Logic

This workflow ensures consistent synchronization of plant-level data
whenever a record is updated.

### Trigger
- The workflow is triggered when a SharePoint item is **created or modified**
- This ensures updates apply both to new records and existing data changes

### Update Item Action
- The workflow uses **Update item** to write values back to the same
  SharePoint list
- Multiple plant-specific fields are updated in a single action

### Field Mapping
- Each plant value column is explicitly mapped
- Examples include:
  - CO Value
  - MN Value
  - PN Value
  - SH Value
  - WI Value
  - HN Value
  - HC Value
  - NCP Value
  - RCP Value
  - SCP Value

This explicit mapping ensures:
- No accidental overwrites
- Clear column-level control
- Predictable data behavior

### Execution Behavior
- Runs automatically upon any change to the item
- Applies updated values immediately
- Ensures consistency across all related plant columns

### Key Technical Considerations
- Event-driven execution to maintain data freshness
- Single update action to reduce flow complexity
- Explicit field mapping for data governance and traceability
