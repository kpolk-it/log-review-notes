# False Positive Notes

Not every alert is a true security incident. These notes help with first-pass judgment.

## Common noisy events
- A user typed the wrong password
- A cached password on a phone or laptop failed
- A service account retried a saved credential
- An expected account lockout after a password change

## When it may still be worth escalating
- Many failures in a short time
- Failures from unusual locations
- Failures against multiple accounts
- A lockout plus unusual successful logon afterward
- A new account created outside change control
- An enabled account that should have stayed disabled

## Documentation tip
If you believe an event is expected, write why.  
Example: "User confirmed recent password change; failures came from their usual workstation."
