# Learner Taking an Assessment – State Diagram

This diagram shows the typical flow a learner follows when taking an assessment in the **Math Booster** system.

```mermaid
stateDiagram-v2
  [*] --> LoggedIn : Learner Logged In
  LoggedIn --> OpenAssessmentList : View Available Assessments
  OpenAssessmentList --> SelectAssessment : Select an Assessment
  SelectAssessment --> ReadInstructions : Read Instructions
  ReadInstructions --> StartAssessment : Click Start
  StartAssessment --> AnswerQuestions : Answer Questions
  AnswerQuestions --> SubmitAssessment : Submit Answers
  SubmitAssessment --> Confirmation : Submission Confirmation
  Confirmation --> [*] : End

### This state diagram maps the begin assessment functional requirement number 5
