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
1. Teacher accesses the course management section
2. Teacher selects the assignment to grade
3. Teacher views list of student submissions
4. Teacher reviews individual student submissions
5. Teacher assigns grades and provides feedback
6. Teacher saves grades for each submission
7. System updates gradebook and notifies students of grades

## Alternative Flows
- **Auto-grading available**: System may pre-grade objective questions
- **Rubric available**: Teacher can use predefined grading rubric

## Exception Flows
- System failure during grading: Error message displayed, grades saved if possible
- File access issues: Alternative methods for reviewing submissions

## Business Rules
- Grades must be within defined range for the assignment
- Feedback must meet quality standards for student learning
- Graded assignments must be released within reasonable timeframe