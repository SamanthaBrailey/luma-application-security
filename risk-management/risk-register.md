# Initial Risk Register

Scores are preliminary and should be updated after testing. Priority combines likelihood and impact rather than relying only on a scanner severity.

| ID | Risk | Likelihood | Impact | Priority | Status |
|---|---|---|---|---|---|
| LUMA-01 | Account takeover through credential stuffing | High | High | Critical | Review planned |
| LUMA-02 | Broken object-level authorization exposes user data | Medium | High | High | Test planned |
| LUMA-03 | Weak password-reset process enables account takeover | Medium | High | High | Test planned |
| LUMA-04 | Malicious or unsafe file upload | Medium | High | High | Test planned |
| LUMA-05 | Application secret committed to source control | Medium | High | High | Review planned |
| LUMA-06 | Stored script injection through user content | Medium | High | High | Test planned |
| LUMA-07 | Excessive collection or retention of personal data | Medium | Medium | Medium | Review planned |
| LUMA-08 | Missing rate limits enable spam or scraping | High | Medium | High | Test planned |
| LUMA-09 | Vulnerable third-party dependency | Medium | Medium | Medium | Scan planned |
| LUMA-10 | Insufficient security logs delay incident response | Medium | High | High | Review planned |

## Risk-review notes

- A listed risk is not a confirmed vulnerability.
- Findings should be supported by repeatable, authorized tests.
- Public documentation should describe remediation without exposing production secrets or a usable attack path.

