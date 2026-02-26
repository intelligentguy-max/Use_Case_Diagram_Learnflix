# UC11 - Create Course

## Use Case Description
Allows teachers to create new courses with structured content, syllabus, and learning materials.

## Actors
- Teacher

## Pre-conditions
- User must be logged in as a Teacher
- Teacher must have appropriate permissions to create courses
- System must be operational

## Post-conditions
- New course is created and stored in the system
- Course appears in teacher's course list
- Course is available for student enrollment (if published)

## Main Flow
1. Teacher accesses course management section
2. Teacher selects option to create a new course
3. Teacher fills in course details (title, description, objectives, etc.)
4. Teacher sets course parameters (enrollment limits, prerequisites, etc.)
5. Teacher adds initial content or syllabus
6. Teacher saves and publishes the course
7. System creates the course and makes it available according to settings

## Alternative Flows
- **Insufficient permissions**: System displays permission error
- **Course already exists**: System alerts teacher of duplicate course

## Exception Flows
- System failure during creation: Error message displayed, partial data saved if possible
- Validation errors: System prompts teacher to correct information

## Business Rules
- Course titles must be unique within the system
- Teachers can only create courses within their authorized subjects
- Course creation requires approval in some configurations