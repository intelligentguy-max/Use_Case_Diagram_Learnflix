# UC09 - Receive Certificate

## Use Case Description
Allows students to access and download certificates upon successful completion of courses.

## Actors
- Student

## Pre-conditions
- User must be logged in as a Student
- Student must have completed all requirements for a course
- Course must have certificate generation enabled
- Grade/marks threshold must be met

## Post-conditions
- Certificate is generated and made available to student
- Completion is recorded in the system
- Student can download or share the certificate

## Main Flow
| User Action | System Response |
|-------------|-----------------|
| Student completes all course requirements | System evaluates completion criteria and grade thresholds |
| | System generates certificate if requirements are met |
| | System notifies student about certificate availability |
| Student accesses the certificate from their dashboard | System displays the available certificate |
| Student downloads or shares the certificate | System provides download/share options |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Requirements not met | Student attempts to access certificate without meeting requirements | System continues to show incomplete status |
| Certificate generation delayed | Student accesses certificate before generation | System displays pending status |

## Exception Flows
- Certificate generation failure: Error handling and retry mechanism
- Download failure: Appropriate error message and retry option

## Business Rules
- Certificates are only issued upon meeting all course requirements
- Certificate templates must be pre-defined and approved
- Digital certificates may include security features to prevent tampering