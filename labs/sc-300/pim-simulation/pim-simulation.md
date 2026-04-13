# Privileged Identity Management (PIM) Simulation

## Objective
Simulate Privileged Identity Management (PIM) in Microsoft Entra ID to demonstrate how organizations secure administrative access using just-in-time (JIT) role activation.

---

## Scenario — Admin Access Should Not Be Permanent

In a traditional Role-Based Access Control (RBAC) setup, administrative roles are assigned permanently.

This creates security risks such as:
- Unauthorized access if an account is compromised  
- Excessive permissions beyond job requirements  
- Increased attack surface for privileged accounts  

---

## Current State (RBAC Implementation)

In previous labs, administrative access was assigned using RBAC.

Example:
- User assigned **User Administrator** role  
- Role remains active at all times  

---

## Problem Identified

- User has continuous administrative access  
- No approval required for elevated privileges  
- No expiration or time restriction on access  

---

## Security Risk

Permanent admin roles violate the principle of least privilege.

If compromised:
- Attacker gains full administrative control  
- No time limits reduce detection opportunities  
- Increased risk of system compromise  

---

## Solution — Privileged Identity Management (PIM)

PIM introduces controlled, temporary access to privileged roles.

---

## Simulated PIM Workflow

### Step 1 — Assign Eligible Role
- User is assigned as **eligible**, not active  
- No admin access by default  

---

### Step 2 — Request Activation
- User must request access when needed  
- Justification may be required  

---

### Step 3 — Temporary Access Granted
- Role becomes active for a limited time (example: 1 hour)  

---

### Step 4 — Automatic Expiration
- Access is removed after time expires  
- User returns to standard permissions  

---

## RBAC vs PIM Comparison

| Feature | RBAC | PIM |
|--------|------|-----|
| Access Type | Always Active | Temporary |
| Security Level | Lower | Higher |
| Risk Exposure | High | Reduced |
| Access Control | Static | Dynamic |

---

## Key Takeaway

This lab demonstrates how traditional RBAC models create security risks through permanent privileged access, and how Privileged Identity Management (PIM) enforces just-in-time access, least privilege, and time-bound permissions to significantly reduce the risk of account compromise and improve overall security posture.

This approach aligns with Zero Trust principles by eliminating standing administrative access and requiring verification and authorization for every privileged action.


---

## Real-World Application

Organizations use PIM to:
- Protect admin accounts  
- Reduce insider threats  
- Improve compliance  
- Control access to critical systems  

---

## Lab Limitation

Privileged Identity Management (PIM) requires a Microsoft Entra ID P2 or Governance license, which was not available in this lab environment.

Due to this limitation, direct configuration of eligible role assignments and just-in-time activation could not be performed.

However, the current RBAC configuration was analyzed, and a secure PIM-based access model was designed and documented to demonstrate how privileged access would be implemented in a real-world enterprise environment.
### PIM License Restriction
![PIM License Restriction](/screenshots/pim-license-restriction.png)

### Risk:
- Permanent admin access increases the risk of account compromise  
- No tracking or approval for privileged actions  
- Violates least privilege principle  

### PIM Solution:
- Admin users are assigned as **eligible** instead of active  
- Access must be requested and justified  
- Access is granted temporarily (e.g., 1 hour)  
- All activation activity is logged for auditing  

### Outcome:
- Reduced attack surface  
- Improved security monitoring  
- Enforced least privilege  
- Better compliance and audit readiness  
---

## Skills Demonstrated

- Identity and Access Management (IAM)  
- RBAC vs PIM understanding  
- Security risk analysis  
- Privileged access concepts

## Security Insight

Privileged accounts are a primary target in cyberattacks.

By eliminating standing administrative access and requiring just-in-time activation, PIM significantly reduces the risk of unauthorized access and limits the impact of compromised credentials.
## Screenshots

### Current RBAC Role Assignment
![RBAC Role](/screenshots/current-rbac-role-assignment.png)

### User Administrator Role Assignments
![Role Page](/screenshots/user-administrator-role-page.png)

### PIM Entry Point
![PIM Entry](/screenshots/pim-entry-point.png)

### PIM License Restriction
![PIM License](/screenshots/pim-license-restriction.png)
