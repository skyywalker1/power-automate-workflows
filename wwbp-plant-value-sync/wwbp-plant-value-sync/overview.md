## Workflow Overview

**Name:** WWBP – Plant Value Sync  
**Platform:** Power Automate  
**Trigger:** When an item is created or modified (SharePoint)

### Business Problem
Plant-level values were being maintained across multiple fields and
were not always synchronized consistently. Manual updates increased the
risk of data mismatches, incomplete records, and unreliable reporting
downstream.

Inconsistent plant values made it difficult to trust aggregated metrics
and required additional manual validation.

### Solution
This workflow automatically updates plant-specific value fields whenever
a SharePoint item is created or modified. The automation ensures that all
related plant value columns are kept in sync based on the latest update.

By standardizing how plant data is written, the workflow improves data
accuracy and reliability for reporting and analysis.

### Data Sources
- SharePoint Online list (WWBP / plant tracking data)
- Multiple plant-specific value columns
