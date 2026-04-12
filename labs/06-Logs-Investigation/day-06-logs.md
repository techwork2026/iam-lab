## Day 6 — Sign-In Logs and Security Investigation

### Objective
Simulate real-world IAM investigation scenarios by reviewing user sign-in activity and analyzing authentication logs in Microsoft Entra ID.

---

### Scenario — User Cannot Log In (Log Investigation)

**Ticket:** User reports inability to sign in and requests investigation

---

### Investigation Steps

- Navigated to user profile in Microsoft Entra ID
- Accessed sign-in logs for the user
- Reviewed sign-in activity for the last 24 hours
- Expanded time range to last 7 days for deeper analysis

**Findings:**
- No sign-in activity recorded within selected time ranges
- No successful or failed authentication attempts detected

![Sign-In Logs Overview](../../screenshots/sign-in-logs-overview.png)

---

### Analysis

The absence of sign-in logs indicates that no authentication attempts were made within the selected time range.

This suggests the issue is not related to authentication failure but may be due to:

- The user not attempting to log in
- Incorrect login methods or endpoints
- Activity outside the selected time window

This points to a likely user-side issue rather than an IAM system failure.
---

### Outcome

No authentication failures or access issues were identified within Microsoft Entra ID.

The investigation ruled out IAM-related causes and redirected troubleshooting toward user behavior, login process validation, and credential verification.
---

### Key Takeaway

This lab demonstrates how sign-in logs are used to investigate authentication issues. Even when no activity is present, analyzing logs helps rule out authentication failures and guides further troubleshooting steps.

---

### Skills Demonstrated

- Sign-in log analysis
- Security investigation
- Microsoft Entra ID monitoring
- Authentication troubleshooting
- Analytical thinking and problem-solving

### Security Insight

Sign-in logs are critical for distinguishing between authentication failures and user behavior issues.

Even when no activity is present, logs provide valuable insight that helps eliminate potential root causes and guide further troubleshooting.
