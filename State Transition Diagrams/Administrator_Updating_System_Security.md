### System Security Updates By The System Administrator

```mermaid
stateDiagram
  direction TB
  [*] --> Still
  Still --> s1
  s1 --> [*]
  Still --> s2
  s2 --> [*]
  s1 --> s5
  s5 --> s6
  s6 --> [*]
  Still:System security
  s1:Updates Pending
  s2:exit
  s5:Updates Fullfield
  s6:exit
style s1 fill:#FFD600,color:#FFFFFF
style s2 fill:#FFD500,color:#FFFFFF
style s5 fill:#FFD600,color:#FFFFFF
style s6 fill:#FFD600,color:#FFFFFF

```