# Common Windows Event IDs

These are useful starting points for triage. This is not a complete list.

## 4624 - Successful Logon
A user or process successfully signed in.

**Why it matters:**  
Helps confirm who signed in, when, and from where.

**What to check:**
- Account name
- Logon type
- Source workstation or IP
- Time of the event
- Whether the activity is normal for that user

## 4625 - Failed Logon
A logon attempt failed.

**Why it matters:**  
Can indicate a typo, a forgotten password, or a brute-force attempt.

**What to check:**
- How many failures occurred
- Time window
- Source IP or workstation
- Whether the account later signed in successfully
- Whether the account is now locked

## 4740 - Account Lockout
An account was locked after too many failed attempts.

**Why it matters:**  
Often tied to password issues, but can also be part of an attack.

**What to check:**
- Which workstation or source caused the lockout
- Recent 4625 events
- Whether the user expected the lockout
- Whether other accounts are being targeted

## 4720 - User Account Created
A new user account was created.

**Why it matters:**  
New accounts can be legitimate or a sign of unauthorized activity.

**What to check:**
- Who created the account
- When it was created
- Whether the request was expected
- What groups or privileges were assigned

## 4722 - User Account Enabled
A previously disabled account was enabled.

**Why it matters:**  
Disabled accounts should not be turned back on without a reason.

## 4723 / 4724 - Password Change or Reset
A password was changed or reset.

**Why it matters:**  
Useful when reviewing possible account takeover.

**What to check:**
- Who initiated the change
- Whether the user requested it
- Whether unusual logons happened afterward
