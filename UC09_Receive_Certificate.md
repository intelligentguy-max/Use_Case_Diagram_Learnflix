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
1. Student completes all course requirements
2. System evaluates completion criteria and grade thresholds
3. System generates certificate if requirements are met
4. System notifies student about certificate availability
5. Student accesses the certificate from their dashboard
6. Student can download or share the certificate

## Alternative Flows
- **Requirements not met**: System continues to show incomplete status
- **Certificate generation delayed**: System displays pending status

## Exception Flows
- Certificate generation failure: Error handling and retry mechanism
- Download failure: Appropriate error message and retry option

## Business Rules
- Certificates are only issued upon meeting all course requirements
- Certificate templates must be pre-defined and approved
- Digital certificates may include security features to prevent tampering