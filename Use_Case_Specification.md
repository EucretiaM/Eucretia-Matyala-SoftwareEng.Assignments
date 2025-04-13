# Use Case Specifications

## Use Case 1: Submit  
**Actor:** Learner  
**Preconditions:** Learner is logged in  
**Postconditions:** Submitted keywords will reflect on the learner's profile against Assignment 5  

### Basic Flow:
1. The learner clicks the start button  
2. The learner clicks the finish button when done  
3. The learner clicks the submit button  
4. The system sends OTP numbers to the learner's email address  
5. Learner submits the assessment after OTP is verified by the system  
6. System updates the submission status to "Submitted"

### Alternative Flows:
- Expired OTP will be discarded  
- Late submissions won’t be accepted  

---

## Use Case 2: Edit Assessment  
**Actor:** Learner  
**Preconditions:** Learner is logged in  
**Postconditions:** The assessment is updated  

### Basic Flow:
1. The learner edits their work during the assessment time  
2. After submission, the learner can edit only if the edit status is enabled  
3. The "Edited" flag pops up  

### Alternative Flows:
- Expired OTP will be discarded  

---

## Use Case 3: Upload Assessment  
**Actor:** Educator  
**Preconditions:** Educator is logged in  
**Postconditions:** The assessment becomes available in the system  

### Basic Flow:
1. Educator uploads assessments on the assessment dashboard  
2. Learners are notified via email and classroom notices  

### Alternative Flows:
- Errors in the assessments may require an extension for submission  

---

## Use Case 4: Mark Allocation  
**Actor:** Educator  
**Preconditions:** Educator is logged in  
**Postconditions:** Marks are captured in the system  

### Basic Flow:
1. Educator uploads assessments on the assessment dashboard  
2. Learners are notified via email and classroom notices  

### Alternative Flows:
- Errors in the assessments may require an extension for submission  

---

## Use Case 5: Reports Generation  
**Actor:** Educator  
**Preconditions:** Educator is logged in  
**Postconditions:** Reports are created and saved by the system  

### Basic Flow:
1. Educator creates a formula based on report criteria (e.g., highest to lowest marks, averages, top 10 learners)  
2. Educator creates as many reports as needed  
3. Educator pushes reports to the dashboard  

### Alternative Flows:
- Reports could become corrupted  

---

## Use Case 6: Checking Assignment Marks  
**Actor:** Learner  
**Preconditions:** Learner is logged in  
**Postconditions:** System updates assessment status as "Marked"  

### Basic Flow:
1. Learner accesses the assessment dashboard using an OTP  
2. The system updates the status to "Visited"  
3. Learner can print or share the results  
4. Educators may push results/reports to the dashboard  

---

## Use Case 7: Delete Dormant Users  
**Actor:** System Administrator  
**Preconditions:** System administrator is logged in  
**Postconditions:** System reflects updated number of users  

### Basic Flow:
1. System administrator checks user activity dates  
2. If users are verified as dormant, they are permanently deleted  
3. The database is updated accordingly  

---

## Use Case 8: System Updates  
**Actor:** Software Developer  
**Preconditions:** Software developer is logged in as an administrator  
**Postconditions:** Outdated APIs and broken code snippets are updated  

### Basic Flow:
1. Developer locks the interface during off-peak hours  
2. Developer fixes bugs and applies updates  
3. Tests are run  
4. Documentation is updated  

### Alternative Flows:
- There may be complications during updates  

---
