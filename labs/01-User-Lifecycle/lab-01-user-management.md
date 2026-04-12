# IAM Hands-On Lab Portfolio — Microsoft Entra ID

This repository documents hands-on Identity and Access Management (IAM) labs performed using Microsoft Entra ID.

The goal is to build real-world IAM experience including:
- User lifecycle management
- Group-based access control
- Role-Based Access Control (RBAC)
- Multi-Factor Authentication (MFA)
- Conditional Access concepts

Each lab simulates enterprise IAM scenarios and includes documentation with screenshots for validation.


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

### Real-World Application
This lab simulates standard IAM processes used in enterprise environments, including onboarding, offboarding, and account recovery workflows.

Users created:
- New Employee
- Contractor
- Intern

Lifecycle actions completed:
- Disabled intern account
- Deleted intern account
- Restored intern account

Status: Completed

---

## IAM Lab 01 — User Lifecycle

## Users Created
![Users Created](../../screenshots/users-created.png)

## User Disabled
![User Disabled](../../screenshots/user-disabled.png)

## User Deleted
![User Deleted](../../screenshots/user-deleted.png)

## User Restored
![User Restored](../../screenshots/user-restored.png)

## Key Takeaway

User lifecycle management is a critical IAM function that ensures users have appropriate access throughout their employment.

Improper onboarding or offboarding can lead to:
- Unauthorized access
- Security risks
- Orphaned accounts

This lab demonstrates how identity management directly impacts organizational security.
