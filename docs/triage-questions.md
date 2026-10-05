# First-Pass Log Review Questions

Use these questions when reviewing a log-based alert.

## Identity
- Which account is involved?
- Is this a standard user, service account, or admin account?
- Is the account currently enabled, disabled, or locked?

## Timing
- When did the event happen?
- Is the time unusual for this user?
- Were there multiple related events around the same time?

## Source
- What workstation or IP is listed?
- Is that source expected?
- Are multiple sources involved?

## Behavior
- Did a successful logon happen after failures?
- Was a new account created or changed?
- Did privileges change?
- Does this match a known business process?

## Decision
- Does this look expected?
- Does this need more review?
- Should this be escalated?
