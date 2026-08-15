# Security Assumptions

These assumptions provide a starting point for the assessment. They must be updated to match Luma's actual architecture.

## Application assumptions

- Luma supports user accounts and public or private profiles.
- Users can create and interact with content.
- The application communicates with a backend API and database.
- Passwords or an external identity provider are used for authentication.
- The application may accept image or file uploads.
- Third-party packages and services are used.
- Administrative or moderation capabilities exist or are planned.

## Trust assumptions to validate

- Server-side authorization is enforced for every protected operation.
- Passwords are never stored in plaintext.
- Secrets are stored outside source code and public repositories.
- Transport encryption is enabled in deployed environments.
- User input is validated and safely rendered.
- Uploaded files are checked and stored safely.
- Security-relevant actions produce useful logs.
- Backups do not expose data or secrets.

## Questions for the next review

1. What frontend, backend, database, and hosting services does Luma use?
2. How are users authenticated?
3. What personal information does Luma collect?
4. Are direct messages or private posts supported?
5. Where are images and uploaded files stored?
6. Which third-party APIs and packages are used?
7. How are administrators identified and protected?
8. Is there a development or staging environment for authorized testing?

