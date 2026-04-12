# Day 2 — Groups & Role-Based Access Control (RBAC) 
## Summary

This lab demonstrates how Role-Based Access Control (RBAC) is implemented in Microsoft Entra ID by organizing users into security groups and assigning administrative roles.

The lab simulates real-world IAM operations, including:

- Structuring users by department
- Managing group-based access
- Assigning administrative permissions
- Verifying access through role assignments

This approach reflects how organizations control access at scale while maintaining security and least privilege principles.

This project simulates real-world enterprise IAM operations, including user lifecycle management, access control, and administrative role assignment within Microsoft Entra ID.

## Objective

Organize users into departments using groups and assign administrative roles using RBAC.

---

## Step 1 — Create Groups

Created the following security groups:

- Finance-Team  
- HR-Team  
- IT-Team  

![Groups Created](../../screenshots/groups-created.png)

---

## Step 2 — Assign Users to Groups

Users were assigned to departments:

- ContractorJason → Finance-Team  
- MaryIntern → HR-Team  
- Samantham → IT-Team  

### Finance Team
![Finance Team](../../screenshots/finance-team-members.png)

### HR Team
![HR Team](../../screenshots/hr-team-members.png)

### IT Team
![IT Team](../../screenshots/it-team-members.png)

---

## Step 3 — Assign Administrative Role

Assigned **User Administrator** role to the user:

- ContractorJason  

![Role Assigned](../../screenshots/role-assigned-user-admin.png)

---

## Step 4 — Verify Role Assignment

Confirmed the role is active under the user account.

![Role Confirmation](../../screenshots/user-role-confirmation.png)

---

## Findings

- Group membership organizes users but does not grant permissions by itself  
- Administrative roles must be assigned to provide access  
- RBAC ensures permissions are controlled based on role instead of individual users
- Improper role assignment can lead to over-permissioned accounts, increasing security risk

---

## Outcome

Successfully created department-based groups and applied RBAC roles to control access.

Verified that role assignment is required for users to gain administrative permissions.

---

## Key Takeaway

RBAC is critical in IAM:

- Groups = organization  
- Roles = access  

Both must be configured correctly to ensure proper access control.

## Skills Demonstrated

- Group-based access control
- Role-Based Access Control (RBAC)
- Administrative role assignment
- Identity organization by department
