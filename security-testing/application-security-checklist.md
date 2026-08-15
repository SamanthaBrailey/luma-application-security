# Application Security Checklist

Use `[x]` only after verifying the control in an authorized environment.

## Accounts

- [ ] Passwords are hashed with a suitable password-hashing algorithm.
- [ ] Login and recovery endpoints are rate-limited.
- [ ] Password-reset tokens expire and cannot be reused.
- [ ] Sessions expire and can be revoked.
- [ ] Administrative accounts receive stronger protection.

## Authorization and privacy

- [ ] Authorization is enforced on the server for every protected resource.
- [ ] Private profiles and content cannot be retrieved through direct API requests.
- [ ] Users can understand and control relevant privacy settings.
- [ ] Account deletion and data-retention behavior are documented.

## Content and uploads

- [ ] User content is safely encoded when displayed.
- [ ] File uploads are restricted by size and validated by content.
- [ ] Uploaded files are stored outside executable locations.
- [ ] Abuse reporting and moderation workflows are documented.

## Secrets and dependencies

- [ ] Secrets are stored outside source code.
- [ ] Repository history has been checked for accidental secrets.
- [ ] Dependencies are scanned and updated through a documented process.
- [ ] Production error messages do not expose sensitive internals.

## Detection and recovery

- [ ] Security-relevant events are logged.
- [ ] Logs do not contain passwords, tokens, or unnecessary personal information.
- [ ] Alerts exist for suspicious login and administrative activity.
- [ ] Backups and recovery procedures have been tested.

