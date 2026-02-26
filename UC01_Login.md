# UC01 - Login

## Use Case Description
Allows registered users (Students, Teachers, and Admins) to authenticate and access the LearnFlix system.

## Actors
- Student
- Teacher
- Admin

## Pre-conditions
- User must have a valid account in the system
- System must be operational
- User must have internet connectivity

## Post-conditions
- User is authenticated and granted access to appropriate dashboard
- Session is established for the user

## Main Flow
| User Action | System Response |
|-------------|-----------------|
| User navigates to the login page | System displays the login interface |
| User enters username/email and password | System captures the credentials |
| User clicks the login button | System validates the credentials |
| | System authenticates the user |
| | System redirects user to the appropriate dashboard based on role |
| | Session is established |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Invalid credentials | User enters incorrect username/password | System displays error message and prompts user to re-enter credentials |
| Account locked/disabled | User attempts to log in with locked account | System displays appropriate message |
| Forgot password | User clicks "Forgot Password" link | System redirects user to password reset process |

## Exception Flows
- System failure during authentication: Error message displayed
- Network connectivity issues: Appropriate error handling

## Business Rules
- Password must meet security requirements
- Account lockout after multiple failed attempts
- Session timeout after period of inactivity