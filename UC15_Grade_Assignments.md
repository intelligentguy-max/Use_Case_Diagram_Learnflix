# UC15 - Grade Assignments

## Use Case Description
Allows teachers to review and grade student assignments with feedback and scores.

## Actors
- Teacher

## Pre-conditions
- User must be logged in as a Teacher
- Teacher must have access rights to the specific course
- Assignment must exist and have student submissions
- Student assignments must be submitted and available for grading

## Post-conditions
- Assignment grades are recorded in the system
- Students receive feedback and scores
- Gradebook is updated with new scores

## Main Flow
| User Action | System Response |
|-------------|-----------------|
| Teacher accesses the course management section | System displays course management options |
| Teacher selects the assignment to grade | System loads assignment details and submissions |
| Teacher views list of student submissions | System displays all submitted assignments |
| Teacher reviews individual student submissions | System provides interface for reviewing submissions |
| Teacher assigns grades and provides feedback | System captures grades and feedback |
| Teacher saves grades for each submission | System updates gradebook and notifies students of grades |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Auto-grading available | Teacher selects auto-grade option | System pre-grades objective questions |
| Rubric available | Teacher selects grading rubric | System provides rubric-based grading interface |

## Exception Flows
- System failure during grading: Error message displayed, grades saved if possible
- File access issues: Alternative methods for reviewing submissions

## Business Rules
- Grades must be within defined range for the assignment
- Feedback must meet quality standards for student learning
- Graded assignments must be released within reasonable timeframe