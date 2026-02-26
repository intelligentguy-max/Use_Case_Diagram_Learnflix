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
| User Action | System Response |
|-------------|-----------------|
| Teacher accesses the course management section | System displays course management options |
| Teacher selects the course for the announcement | System loads course-specific management interface |
| Teacher chooses to create a new announcement | System provides announcement composition interface |
| Teacher composes the announcement message | System captures and validates the message |
| Teacher sets visibility and timing preferences | System applies visibility and timing settings |
| Teacher posts the announcement | System distributes notification to enrolled students |
| | System stores the announcement in course communications |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Scheduled announcement | Teacher schedules announcement for future posting | System queues announcement for specified time |
| Targeted announcement | Teacher targets specific student groups | System applies targeted distribution settings |

## Exception Flows
- System failure during posting: Error message displayed
- Network issues: Appropriate error handling

## Business Rules
- Announcements must be relevant to the specific course
- Teachers should follow communication guidelines
- Critical announcements may require acknowledgment from students