# Luma Threat Model

## Assets

- User accounts and authentication sessions
- Personal information and private content
- Public posts, comments, and media
- Administrative privileges
- Application secrets and API keys
- Database integrity and availability
- User trust and platform reputation

## Threat actors

- Automated bots and spammers
- Account thieves using leaked credentials
- Abusive or malicious users
- Attackers targeting the application or API
- Unauthorized insiders or compromised administrators
- Third parties affected by a compromised dependency

## STRIDE review

| Category | Luma example | Possible controls |
|---|---|---|
| Spoofing | Attacker takes over or impersonates an account | MFA, rate limits, secure recovery, session controls |
| Tampering | User changes another user's content through an API request | Server-side authorization, validation, audit logs |
| Repudiation | User denies performing a destructive action | Time-synchronized audit logs and account identifiers |
| Information disclosure | Private messages or profiles become publicly accessible | Access control testing, encryption, data minimization |
| Denial of service | Automated requests exhaust application resources | Rate limits, quotas, caching, monitoring |
| Elevation of privilege | Normal user gains moderator or administrator access | Role checks, least privilege, protected admin workflows |

## Highest-priority scenarios

1. Credential stuffing results in account takeover.
2. An insecure object reference exposes another user's private information.
3. A malicious file upload is stored or executed unsafely.
4. A stolen token allows a session to remain active.
5. An exposed secret grants access to a database or third-party service.
6. Automated accounts generate spam or scrape user data.

