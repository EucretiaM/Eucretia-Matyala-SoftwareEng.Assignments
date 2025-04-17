# Deleting Redundant Data – State Diagram

This diagram represents the flow for deleting redundant data in the **Math Booster** system.

```mermaid
stateDiagram-v2
  [*] --> SystemCheck : Start Redundancy Check
  SystemCheck --> RedundantDataFound : Redundant Data Found?
  RedundantDataFound --> ConfirmDelete : Yes
  RedundantDataFound --> [*] : No

  ConfirmDelete --> DeletingData : Confirm Deletion
  DeletingData --> CleanupComplete : Data Deleted
  CleanupComplete --> [*] : End Process
