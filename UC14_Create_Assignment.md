# UC14 - Create Assignment

## Use Case Description
Allows teachers to create assignments and coursework for students with specific instructions and deadlines.

## Actors
- Teacher

## Pre-conditions
- User must be logged in as a Teacher
- Teacher must have access rights to the specific course
- Course must exist in the system

## Post-conditions
- Assignment is created and stored in the system
- Assignment is associated with the appropriate course
- Assignment availability and deadline settings are configured

## Main Flow
1. Teacher accesses the course management section
2. Teacher selects the course for which to create an assignment
3. Teacher chooses to create a new assignment
4. Teacher defines assignment details (title, description, instructions)
5. Teacher sets assignment parameters (due date, submission format, etc.)
6. Teacher specifies grading criteria and point value
7. Teacher saves and publishes the assignment
8. System stores the assignment and applies the settings

## Alternative Flows
- **Template available**: Teacher can use existing assignment template
- **Group assignment**: Teacher can configure for group submissions

## Exception Flows
- System failure during creation: Error message displayed, partial data saved if possible
- Validation errors: System prompts teacher to correct information

## Business Rules
- Assignment due dates must be in the future
- Submission formats must be clearly defined
- Grading rubrics must be established before assignment publication