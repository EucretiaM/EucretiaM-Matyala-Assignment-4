# Use Case Specification

## Use Case 1: Submit
**Actor:** Learner  
**Preconditions:** Learner is logged in  
**Postconditions:** Submitted keywords will reflect on the learner's profile against assignment 5.  

### Basic Flow:
- The learner clicks the start button.
- The learner clicks the finish button when done.
- The learner clicks the submit button when done.
- The system sends OTP numbers to the learner's email address.
- Learner submits the assessment when OTP has been verified by the system.
- System updates the submission status to "submitted".

### Alternative Flows:
- Expired OTP will be discarded.
- Late submissions won’t be accepted.

---
## Use Case 2: Edit Assessment
**Actor:** Learner  
**Preconditions:** Learner is logged in  
**Postconditions:** The assessment has been updated.  

### Basic Flow:
- The learner edits their work during the assessment time.
- After submission, the learner can edit only if the edit status is available.
- The edited flag pops up.

### Alternative Flows:
- Expired OTP will be discarded.

---
## Use Case 3: Upload Assessment
**Actor:** Educator  
**Preconditions:** Educator is logged in  
**Postconditions:** The assessment is available on the system.  

### Basic Flow:
- Educator uploads assessments on the assessment dashboard.
- Learners will be notified via emails and classroom notices.

### Alternative Flows:
- Errors in the assessments could lead to an extension for submission.

---
## Use Case 4: Mark Allocation
**Actor:** Educator  
**Preconditions:** Educator is logged in  
**Postconditions:** The mark scored will be captured in the system.  

### Basic Flow:
- Educator uploads assessments on the assessment dashboard.
- Learners will be notified via emails and classroom notices.

### Alternative Flows:
- Errors in the assessments could lead to an extension for submission.

---
## Use Case 5: Reports Generation
**Actor:** Educator  
**Preconditions:** Educator is logged in  
**Postconditions:** Reports are created, and the system records them.  

### Basic Flow:
- Educator creates a formula based on the criteria of the reports (e.g., highest to lowest marks, averages, top 10 learners).
- Educator generates as many reports as needed based on the desired criteria.
- Educator pushes the reports to the dashboard.

### Alternative Flows:
- Reports could get corrupted.

---
## Use Case 6: Checking Assignment Marks
**Actor:** Learner  
**Preconditions:** Learner is logged in  
**Postconditions:** System updates assessment status as "marked".  

### Basic Flow:
- Learner logs onto the assessments dashboard via OTP to access their marks.
- The system updates the status to "visited".
- Learner has the option to print or share the results.
- Educators can push the reports to the dashboard.

---
## Use Case 7: Delete Dormant Users
**Actor:** System Administrator  
**Preconditions:** System administrator is logged in  
**Postconditions:** System updates the count of users.  

### Basic Flow:
- The system administrator checks user activity dates.
- If dormant users are verified, permanent deletion is processed.
- The database is updated.

---
## Use Case 8: System Updates
**Actor:** Software Developer  
**Preconditions:** The software developer is logged in as an administrator.  
**Postconditions:** Outdated APIs and broken snippets are updated.  

### Basic Flow:
- The software developer locks the interface during off-peak hours.
- Fixes bugs and updates the system.
- Runs tests.
- Completes documentation.

### Alternative Flows:
- There may be complications during updates.
