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
1. Student navigates to the quiz section of a course
2. System displays available quizzes
3. Student selects a quiz to take
4. System presents quiz questions to the student
5. Student answers questions and submits the quiz
6. System processes and saves the responses
7. System calculates and displays the score (if immediately available)

## Alternative Flows
- **Quiz not available**: System displays appropriate message
- **Time limit exceeded**: System auto-submits or prevents submission
- **Incomplete submission**: System prompts student to complete unanswered questions

## Exception Flows
- System failure during quiz: Responses saved automatically, error message displayed
- Network disconnection: Auto-save functionality activated

## Business Rules
- Quizzes may have time limits
- Responses are saved automatically during quiz
- Scores may be immediately available or delayed based on settings
- Quiz attempts may be limited