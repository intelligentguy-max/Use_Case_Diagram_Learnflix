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
| User Action | System Response |
|-------------|-----------------|
| Teacher accesses the course management section | System displays course management options |
| Teacher selects the course for which to create an assignment | System loads course-specific options |
| Teacher chooses to create a new assignment | System provides assignment creation interface |
| Teacher defines assignment details (title, description, instructions) | System captures and validates assignment details |
| Teacher sets assignment parameters (due date, submission format, etc.) | System processes parameter settings |
| Teacher specifies grading criteria and point value | System stores grading information |
| Teacher saves and publishes the assignment | System stores the assignment and applies the settings |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Template available | Teacher selects existing assignment template | System allows teacher to use existing template |
| Group assignment | Teacher configures for group submissions | System adjusts assignment settings for group work |

## Exception Flows
- System failure during creation: Error message displayed, partial data saved if possible
- Validation errors: System prompts teacher to correct information

## Business Rules
- Assignment due dates must be in the future
- Submission formats must be clearly defined
- Grading rubrics must be established before assignment publication