# Account Takeover Response Playbook

## Purpose

Guide the initial response when a Luma account may have been accessed by an unauthorized person.

## Indicators

- Unusual login location or device
- Repeated failed logins followed by success
- Unexpected password, email, or profile changes
- Spam or messages the user did not create
- Multiple user reports involving similar activity

## Initial response

1. Record the report time, affected account, and available evidence.
2. Preserve relevant authentication and account-change logs.
3. Revoke active sessions and recovery tokens when appropriate.
4. Protect the account from further changes.
5. Help the user reset credentials through a verified recovery process.
6. Determine whether other accounts show the same indicators.

## Investigation questions

- When did suspicious activity begin?
- Which sessions, IP addresses, devices, or user agents were involved?
- Was the password reset or recovery process used?
- Were private messages or personal information accessed?
- Did the compromised account send links, spam, or abusive content?
- Does the pattern suggest credential stuffing or a platform vulnerability?

## Recovery and follow-up

- Restore legitimate account information.
- Notify affected users using an approved communication process.
- Block confirmed malicious indicators when appropriate.
- Fix the control failure that allowed or prolonged the incident.
- Monitor for recurrence.
- Document lessons learned and update detection rules.

## Portfolio tabletop scenario

Simulate three test accounts showing successful logins after repeated failures. Walk through triage, containment, user recovery, evidence preservation, and the decision to check for a wider credential-stuffing campaign. Use synthetic data only.

