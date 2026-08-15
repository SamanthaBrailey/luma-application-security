# Remediation Roadmap

## First 30 days

- Confirm Luma's architecture and data inventory.
- Verify secrets are excluded from source control.
- Review authentication, password reset, and session expiration.
- Test server-side authorization for user-owned resources.
- Enable dependency and secret scanning.
- Define security logging requirements.

## Days 31–60

- Add or tune rate limiting for login, registration, posting, and search.
- Validate file types, content, size, and storage location.
- Review administrative roles and require stronger authentication.
- Document privacy settings and data-deletion behavior.
- Test output encoding and input handling for user-generated content.

## Days 61–90

- Run an account-takeover tabletop exercise.
- Create alerts for repeated login failures and unusual administrative activity.
- Validate backup access and recovery procedures.
- Retest completed fixes.
- Record remaining accepted risks and responsible owners.

## Definition of done

A risk is not considered remediated until the control is implemented, tested, documented, and verified not to break the expected user workflow.

