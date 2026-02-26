# UC06 - Submit Assignment

## Use Case Description
Allows students to submit assignments and coursework to the system for evaluation.

## Actors
- Student

## Pre-conditions
- User must be logged in as a Student
- Student must be enrolled in the course containing the assignment
- Assignment must be active and accepting submissions
- Assignment deadline must not have passed

## Post-conditions
- Assignment submission is recorded in the system
- Submission timestamp is captured
- Assignment status is updated

## Main Flow
| User Action | System Response |
|-------------|-----------------|
| Student navigates to the assignment section of a course | System displays available assignments |
| Student selects an assignment to submit | System provides submission interface |
| Student uploads assignment files or completes online assignment | System validates file format and size |
| Student submits the assignment | System records the submission with timestamp |
| | System updates assignment status to submitted |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Deadline passed | Student attempts to submit after deadline | System displays message and prevents submission |
| File size limit exceeded | Student uploads oversized file | System displays error message |
| Invalid file format | Student uploads unsupported file type | System displays appropriate error |

## Exception Flows
- Upload failure: Error message displayed, opportunity to retry
- System failure during submission: Error handling with recovery options

## Business Rules
- Submissions are timestamped upon receipt
- File size and format restrictions apply
- Late submissions may be rejected or marked accordingly
- Students may be allowed multiple attempts (configurable)