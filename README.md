# Luma Application Security Project

Luma is a social media application I built with AI-assisted development tools. This repository focuses on how I would protect the application and its users rather than presenting the application as a coding project.

My security review looks at authentication, account abuse, sensitive data, user-generated content, API security, third-party dependencies, logging, and incident response. Where testing has not yet been completed, the item is marked as planned instead of being presented as a verified result.

## Project goals

- Identify the information and features that need protection.
- Document realistic threats against a social media application.
- Prioritize security risks by likelihood and impact.
- Recommend preventive and detective controls.
- Create a repeatable security-testing plan.
- Explain how I would respond to a security incident affecting Luma.

## Repository contents

```text
luma-application-security/
├── README.md
├── architecture/
│   ├── data-flow.md
│   └── security-assumptions.md
├── threat-model/
│   ├── abuse-cases.md
│   └── threat-model.md
├── risk-management/
│   ├── remediation-roadmap.md
│   └── risk-register.md
├── security-testing/
│   ├── application-security-checklist.md
│   └── testing-plan.md
└── incident-response/
    └── account-takeover-playbook.md
```

## Security scope

The initial assessment covers:

- Account registration, login, logout, and password reset
- User profiles and privacy settings
- Posts, comments, likes, follows, and direct messages if supported
- File and image uploads
- Application APIs
- Administrative and moderation functions
- Logs, alerts, backups, and third-party services

The exact architecture and implemented controls must be confirmed against the current Luma application before testing.

## Main security concerns

1. **Account takeover** through weak authentication, credential stuffing, or insecure password reset.
2. **Broken authorization** that lets one user view or change another user's private data.
3. **Injection and unsafe input handling** in posts, comments, search fields, and APIs.
4. **Malicious uploads** disguised as images or other permitted files.
5. **Privacy exposure** involving profiles, messages, location data, or deleted content.
6. **Platform abuse** such as spam, impersonation, harassment, scraping, and automated account creation.
7. **Dependency and secret exposure** in packages, source control, logs, or deployment settings.
8. **Insufficient monitoring** that delays the discovery of suspicious activity.

## Current status

| Area | Status |
|---|---|
| Security assumptions | Drafted |
| Data-flow review | Drafted; architecture validation needed |
| Threat model | Drafted |
| Risk register | Drafted |
| Security testing | Planned |
| Remediation validation | Not started |
| Incident-response exercise | Planned |

## Planned evidence

As testing is completed, this repository can include sanitized evidence such as:

- A data-flow diagram
- Authentication and authorization test results
- Dependency-scan summary
- Redacted screenshots of security settings or test results
- Before-and-after remediation comparisons
- A short incident-response tabletop exercise

No passwords, tokens, private user data, production secrets, or exploitable production details should be committed.

## AI-assisted development disclosure

I used Cursor as a development assistant while building Luma. This security project documents my own review of the application's risks, security decisions, testing process, and remediation priorities. AI-generated suggestions must be reviewed and validated before being treated as implemented or secure.

## Ethical testing statement

Security testing should be limited to application instances, accounts, and data that I own or am explicitly authorized to test. Destructive testing and tests involving real user data are outside the scope of this portfolio project.

