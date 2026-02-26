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
| User Action | System Response |
|-------------|-----------------|
| Student browses available courses | System displays list of available courses |
| Student selects a course for enrollment | System checks prerequisites and availability |
| Student confirms enrollment request | System processes enrollment request |
| | System confirms enrollment and updates student's course list |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Prerequisites not met | Student attempts to enroll without meeting prerequisites | System displays message and suggests alternative actions |
| Course full | Student attempts to enroll in a full course | System displays message and offers waitlist option if available |
| Already enrolled | Student attempts to enroll in an already enrolled course | System displays appropriate message |

## Exception Flows
- System failure during enrollment: Transaction rolled back, error message displayed
- Network issues: Appropriate error handling

## Business Rules
- Students can only enroll in courses with available capacity
- Prerequisites must be satisfied before enrollment
- Maximum number of courses per student may be limited