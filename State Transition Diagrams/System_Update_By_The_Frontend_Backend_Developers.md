# System Update by Frontend & Backend Developers – State Diagram

This diagram outlines the update process followed by frontend and backend developers when maintaining or enhancing the Math Booster system.

```mermaid
stateDiagram-v2
  [*] --> PlanUpdate : Plan Update
  PlanUpdate --> AssignTasks : Assign Tasks (Frontend/Backend)
  AssignTasks --> DevWork : Implement Code Changes
  DevWork --> CommitCode : Commit & Push to Repository
  CommitCode --> CodeReview : Code Review & Testing
  CodeReview --> ChangesRequired : Request Changes?
  ChangesRequired --> DevWork : Yes – Make Revisions
  ChangesRequired --> MergeCode : No – Approve Merge
  MergeCode --> DeployToStaging : Deploy to Staging
  DeployToStaging --> FinalTesting : Perform Final Testing
  FinalTesting --> DeployToProduction : Approve for Production
  DeployToProduction --> [*] : Update Complete
