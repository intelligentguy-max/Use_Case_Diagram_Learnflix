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
1. Teacher accesses the course management section
2. Teacher selects the course for which to create a quiz
3. Teacher chooses to create a new quiz
4. Teacher configures quiz settings (time limit, attempts allowed, etc.)
5. Teacher adds questions with correct answers and scoring
6. Teacher sets quiz availability dates and conditions
7. Teacher saves and publishes the quiz
8. System stores the quiz and applies the settings

## Alternative Flows
- **Insufficient permissions**: System displays permission error
- **Question bank available**: Teacher can select from existing questions

## Exception Flows
- System failure during creation: Error message displayed, partial data saved if possible
- Validation errors: System prompts teacher to correct information

## Business Rules
- Quiz questions must have clear correct answers for automatic grading
- Time limits and attempt restrictions must be clearly defined
- Quizzes may be scheduled to open/close automatically