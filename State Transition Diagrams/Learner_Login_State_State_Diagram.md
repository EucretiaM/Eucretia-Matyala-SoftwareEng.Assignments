# Learner Login State Diagram

This state diagram represents the learner login flow in the **Math Booster** system.

```mermaid
stateDiagram-v2
  [*] --> OpeningApp : Open App
  OpeningApp --> EnteringCredentials : Enter Credentials
  EnteringCredentials --> VerifyingLogin : Click Login
  VerifyingLogin --> AccessDenied : Incorrect Credentials
  VerifyingLogin --> Dashboard : Correct Credentials
  AccessDenied --> EnteringCredentials : Try Again
  Dashboard --> [*] : Logout

