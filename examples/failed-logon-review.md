# Example: Failed Logon Review

**Scenario:** Several 4625 events were recorded for one user account.

### What Was Reviewed
- Number of failed attempts
- Time range
- Source workstation
- Whether a 4624 successful logon followed
- Whether the account was locked

### Findings
- Five failed attempts occurred over three minutes
- Source was the user’s normal workstation
- User later signed in successfully
- Account was not locked

### Decision
Likely a password typo. Documented and closed with notes. No escalation required.

### Why This Matters
This shows the difference between a small number of local failures and a possible brute-force pattern.

