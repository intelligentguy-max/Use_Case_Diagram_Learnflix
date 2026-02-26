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
1. Admin accesses the system administration section
2. Admin selects the permission management interface
3. Admin chooses to modify permissions for a specific role or user
4. Admin configures access rights and permissions
5. Admin saves the permission settings
6. System applies the new permissions
7. System updates access controls and logs the changes

## Alternative Flows
- **Role-based permissions**: Admin can set permissions for entire user roles
- **Individual permissions**: Admin can override role permissions for specific users

## Exception Flows
- System failure during permission update: Error message displayed, rollback if needed
- Security validation errors: System prevents potentially harmful permission changes

## Business Rules
- Principle of least privilege must be followed
- Administrative permissions should be carefully controlled
- Permission changes should be auditable and reversible