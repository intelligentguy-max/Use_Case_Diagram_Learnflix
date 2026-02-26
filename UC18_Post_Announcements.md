# UC18 - Post Announcements

## Use Case Description
Allows teachers to communicate important information, updates, and announcements to students in their courses.

## Actors
- Teacher

## Pre-conditions
- User must be logged in as a Teacher
- Teacher must have access rights to the specific course
- Course must exist and have enrolled students

## Post-conditions
- Announcement is posted to the course
- Students are notified of the new announcement
- Announcement is stored in course communication history

## Main Flow
1. Teacher accesses the course management section
2. Teacher selects the course for the announcement
3. Teacher chooses to create a new announcement
4. Teacher composes the announcement message
5. Teacher sets visibility and timing preferences
6. Teacher posts the announcement
7. System distributes notification to enrolled students
8. System stores the announcement in course communications

## Alternative Flows
- **Scheduled announcement**: Teacher can schedule announcement for future posting
- **Targeted announcement**: Teacher can target specific student groups

## Exception Flows
- System failure during posting: Error message displayed
- Network issues: Appropriate error handling

## Business Rules
- Announcements must be relevant to the specific course
- Teachers should follow communication guidelines
- Critical announcements may require acknowledgment from students