# Lab 01 — User Lifecycle Management

## Objective
Simulate employee onboarding and offboarding using Microsoft Entra ID.

This lab demonstrates:

- Creating users
- Assigning basic profile info
- Disabling accounts
- Deleting users
- Restoring users

---

## Scenario

A company hires three new users:

- New Employee
- Contractor
- Intern

Each user will be created, modified, and offboarded.

---

## Step 1 — Create Users

Users created:

| Name | Role | Department | Status |
|------|------|------------|--------|
| John Employee | Full Time | IT | Active |
| Sarah Contractor | Contractor | Finance | Active |
| Mike Intern | Intern | HR | Active |

---

## Step 2 — Disable User

Contractor account disabled after project completion.

---

## Step 3 — Delete User

Intern account deleted after internship.

---

## Step 4 — Restore User

Intern account restored from deleted users.

---

## Skills Demonstrated

- Microsoft Entra ID
- User lifecycle management
- Identity governance basics
- Account recovery

## Result

Users created:
- New Employee
- Contractor
- Intern

Lifecycle actions completed:
- Disabled intern account
- Deleted intern account
- Restored intern account

Status: Completed
# IAM Lab 01 — User Lifecycle

## Users Created
![Users Created](screenshots/users-created.png)

## User Disabled
![User Disabled](screenshots/user-disabled.png)

## User Deleted
![User Deleted](screenshots/user-deleted.png)

## User Restored
![User Restored](screenshots/user-restored.png)




---

# Day 2 — Groups & Role-Based Access Control (RBAC) 
## Summary

This lab demonstrates hands-on Identity and Access Management (IAM) using Microsoft Entra ID.

Key tasks performed:

- Created and managed user accounts
- Organized users into department-based groups
- Implemented Role-Based Access Control (RBAC)
- Assigned administrative roles to users
- Verified role-based permissions

This project simulates real-world enterprise IAM operations, including user lifecycle management, access control, and administrative role assignment within Microsoft Entra ID.

## Objective

Organize users into departments using groups and assign administrative roles using RBAC.

---

## Step 1 — Create Groups

Created the following security groups:

- Finance-Team
- HR-Team
- IT-Team

![Groups Created](./screenshots/groups-created.png)

---

## Step 2 — Assign Users to Groups

Users were assigned to departments:

- ContractorJason → Finance-Team  
- Maryintern → HR-Team  
- Samantham → IT-Team  

### Finance Team
![Finance Team](./screenshots/finance-team-members.png)

### HR Team
![HR Team](./screenshots/hr-team-members.png)

### IT Team
![IT Team](./screenshots/it-team-members.png)

---

## Step 3 — Assign Administrative Role

Assigned **User Administrator** role to:

- ContractorJason

![Role Assigned](./screenshots/role-assigned-user-admin.png)

---

## Step 4 — Verify Role Assignment

Confirmed the role is active under the user account.

![Role Confirmation](./screenshots/user-role-confirmation.png)

---

## Skills Demonstrated

- Group-based access control
- Role-Based Access Control (RBAC)
- Administrative role assignment
- Identity organization by department


---

# Day 3 — Conditional Access (MFA Enforcement)

## Step 1 — Access Conditional Access

Navigated to:

Microsoft Entra ID → Security → Conditional Access

Attempted to create a new policy.

---

## Step 2 — Policy Creation (Simulated)

Due to Microsoft Entra ID Free tier limitations, Conditional Access policy creation is not available.

The following policy was designed:

**Policy Name:** Require MFA for All Users

**Assignments:**
- All Users

**Cloud Apps:**
- All cloud apps

**Access Controls:**
- Require Multi-Factor Authentication (MFA)

This policy enforces MFA across the organization.

![Conditional Access Not Available](./screenshots/conditional-access-not-available.png)


## Day 3 — MFA and Conditional Access

### Objective
Today I explored multi-factor authentication (MFA) settings in Microsoft Entra ID and checked Conditional Access availability in the lab environment.

### What I did
- Opened Microsoft Entra admin center
- Navigated to user authentication settings
- Reviewed available MFA method options
- Checked Conditional Access availability
- Documented limitations shown in the lab tenant

### Key takeaway
This lab showed how MFA settings can be reviewed and managed for users, while also confirming that some Conditional Access features may not be available depending on licensing or lab environment configuration.
This demonstrates hands-on experience navigating Microsoft Entra ID, reviewing authentication methods, and identifying access control limitations within a lab tenant.

### Skills Demonstrated
- Identity and Access Management (IAM)
- Multi-Factor Authentication (MFA)
- Microsoft Entra ID navigation
- Access control analysis
- Documentation and audit tracking

### Screenshots

#### Conditional Access unavailable (lab limitation)
![Conditional Access not available](screenshots/conditional-access-not-available.png)

#### MFA method options
![MFA method options](screenshots/mfa-method-options.png)

#### MFA methods for user
![MFA methods for user](screenshots/mfa-methods-user.png)
