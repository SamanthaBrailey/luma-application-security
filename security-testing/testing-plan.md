# Security Testing Plan

## Rules of engagement

- Test only an owned or explicitly authorized Luma environment.
- Use dedicated test accounts and synthetic data.
- Avoid destructive tests against production.
- Stop if testing affects real users or system availability.
- Record dates, scope, tools, observations, and remediation status.

## Planned tests

### Authentication

- Confirm login responses do not reveal whether an account exists.
- Verify password-reset tokens expire and cannot be reused.
- Check session expiration and logout behavior.
- Confirm sensitive account changes require appropriate verification.
- Review protections against repeated login attempts.

### Authorization

- Attempt to access another test user's profile, posts, messages, and settings by changing identifiers.
- Confirm privileged endpoints reject normal users.
- Verify private content remains private through both the interface and direct API requests.

### Input and content

- Test special characters and markup in posts, comments, profiles, and search fields.
- Confirm output is safely encoded.
- Validate upload size, extension, content type, filename, and storage behavior.

### API and configuration

- Review cross-origin settings and error messages.
- Confirm secrets are not present in client bundles, repositories, or logs.
- Run dependency and secret scans.
- Review security headers in the deployed test environment.

### Monitoring

- Confirm failed logins, password resets, account changes, and administrator actions are logged.
- Check whether logs contain enough context without storing passwords or tokens.
- Define alert thresholds for suspicious activity.

## Evidence format

For each completed test, record:

- Test ID and date
- Authorized environment
- Expected result
- Observed result
- Sanitized evidence
- Risk rating
- Recommended fix
- Retest result

