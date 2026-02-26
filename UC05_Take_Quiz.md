# UC05 - Take Quiz

## Use Case Description
Allows students to participate in quizzes and assessments within courses.

## Actors
- Student

## Pre-conditions
- User must be logged in as a Student
- Student must be enrolled in the course containing the quiz
- Quiz must be active and available for submission
- Quiz time window must be open (if applicable)

## Post-conditions
- Student's quiz responses are recorded
- Quiz score is calculated and stored
- Progress is updated in the system

## Main Flow
| User Action | System Response |
|-------------|-----------------|
| Student navigates to the quiz section of a course | System displays available quizzes |
| Student selects a quiz to take | System presents quiz questions to the student |
| Student answers questions and submits the quiz | System processes and saves the responses |
| | System calculates and displays the score (if immediately available) |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Quiz not available | Student attempts to access inactive quiz | System displays appropriate message |
| Time limit exceeded | Student continues after time limit | System auto-submits or prevents submission |
| Incomplete submission | Student attempts to submit without answering all questions | System prompts student to complete unanswered questions |

## Exception Flows
- System failure during quiz: Responses saved automatically, error message displayed
- Network disconnection: Auto-save functionality activated

## Business Rules
- Quizzes may have time limits
- Responses are saved automatically during quiz
- Scores may be immediately available or delayed based on settings
- Quiz attempts may be limited