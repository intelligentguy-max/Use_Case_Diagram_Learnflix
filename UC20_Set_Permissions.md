# UC20 - Set Permissions

## Use Case Description
Allows administrators to configure and manage system permissions and access controls for different user roles.

## Actors
- Admin

## Pre-conditions
- User must be logged in as an Admin
- Admin must have appropriate permissions for permission management
- System must be operational

## Post-conditions
- System permissions are updated according to admin configuration
- User access rights are modified based on new permissions
- Permission changes are logged in the system

## Main Flow
| User Action | System Response |
|-------------|-----------------|
| Admin accesses the system administration section | System displays administration options |
| Admin selects the permission management interface | System provides permission management tools |
| Admin chooses to modify permissions for a specific role or user | System loads current permissions for selected role/user |
| Admin configures access rights and permissions | System captures and validates permission changes |
| Admin saves the permission settings | System applies the new permissions |
| | System updates access controls and logs the changes |

## Alternative Flows
| Condition | User Action | System Response |
|-----------|-------------|-----------------|
| Role-based permissions | Admin sets permissions for entire user roles | System applies permissions to all users in selected role |
| Individual permissions | Admin overrides role permissions for specific users | System applies individual permissions overriding role defaults |

## Exception Flows
- System failure during permission update: Error message displayed, rollback if needed
- Security validation errors: System prevents potentially harmful permission changes

## Business Rules
- Principle of least privilege must be followed
- Administrative permissions should be carefully controlled
- Permission changes should be auditable and reversible