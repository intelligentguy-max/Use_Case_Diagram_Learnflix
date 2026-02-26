# UC13 - Create Quiz

## Use Case Description
Allows teachers to create quizzes and assessments for their courses with various question types and settings.

## Actors
- Teacher

## Pre-conditions
- User must be logged in as a Teacher
- Teacher must have access rights to the specific course
- Course must exist in the system

## Post-conditions
- Quiz is created and stored in the system
- Quiz is associated with the appropriate course
- Quiz availability settings are configured

## Main Flow
| User Action | System Response |
|-------------|-----------------|
| Teacher accesses the course management section | System displays course management options |
| Teacher selects the course for which to create a quiz | System loads course-specific options |
| Teacher chooses to create a new quiz | System provides quiz creation interface |
| Teacher configures quiz settings (time limit, attempts allowed, etc.) | System captures and validates settings |
| Teacher adds questions with correct answers and scoring | System processes and stores questions |
| Teacher sets quiz availability dates and conditions | System applies availability settings |
| Teacher saves and publishes the quiz | System stores the quiz and applies the settings |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Insufficient permissions | Teacher attempts to create quiz without proper permissions | System displays permission error |
| Question bank available | Teacher selects existing questions | System allows selection from question bank |

## Exception Flows
- System failure during creation: Error message displayed, partial data saved if possible
- Validation errors: System prompts teacher to correct information

## Business Rules
- Quiz questions must have clear correct answers for automatic grading
- Time limits and attempt restrictions must be clearly defined
- Quizzes may be scheduled to open/close automatically