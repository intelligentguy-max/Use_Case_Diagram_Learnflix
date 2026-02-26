# UC03 - Enroll in Course

## Use Case Description
Allows students to enroll in available courses based on prerequisites and availability.

## Actors
- Student

## Pre-conditions
- User must be logged in as a Student
- Course must be available for enrollment
- Prerequisites (if any) must be met

## Post-conditions
- Student is enrolled in the selected course
- Course appears in student's course list
- Enrollment is recorded in the system

## Main Flow
1. Student browses available courses
2. Student selects a course for enrollment
3. System checks prerequisites and availability
4. System processes enrollment request
5. System confirms enrollment and updates student's course list

## Alternative Flows
- **Prerequisites not met**: System displays message and suggests alternative actions
- **Course full**: System displays message and offers waitlist option if available
- **Already enrolled**: System displays appropriate message

## Exception Flows
- System failure during enrollment: Transaction rolled back, error message displayed
- Network issues: Appropriate error handling

## Business Rules
- Students can only enroll in courses with available capacity
- Prerequisites must be satisfied before enrollment
- Maximum number of courses per student may be limited