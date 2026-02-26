# UC08 - Participate in Discussions

## Use Case Description
Allows students to engage in course-related discussions and forums.

## Actors
- Student

## Pre-conditions
- User must be logged in as a Student
- Student must be enrolled in the course containing the discussion forum
- Discussion forum must be active and enabled

## Post-conditions
- Student's participation is recorded in the system
- Discussion posts and replies are stored
- Engagement metrics are updated

## Main Flow
1. Student navigates to the discussion forum of a course
2. System displays discussion threads and topics
3. Student selects a topic or creates a new thread
4. Student posts a message or replies to existing posts
5. System validates and stores the post
6. System updates discussion activity and notifies relevant participants

## Alternative Flows
- **Forum not active**: System displays appropriate message
- **Restricted posting**: System enforces posting rules and restrictions

## Exception Flows
- Post submission failure: Error message displayed with retry option
- Network issues: Appropriate error handling

## Business Rules
- Posts must comply with community guidelines
- Moderation may be applied to posts before visibility
- Students can reply to their own and others' posts within course boundaries