# Security Controls

| Control Area | Portfolio Approach | Intended Purpose |
|---|---|---|
| Identity | AWS IAM / role-based access | Restrict access according to responsibilities |
| Authorization | Least privilege | Minimize unnecessary permissions |
| Network access | Security Groups | Control permitted traffic |
| Data protection | Encryption at rest and in transit | Protect data confidentiality |
| Monitoring | AWS CloudTrail | Record account/API activity |
| Auditability | Audit logging | Support traceability and review |

## Architecture Decision
Security is treated as an architectural requirement rather than an add-on. Access, encryption, and monitoring controls are incorporated into the proposed design.
