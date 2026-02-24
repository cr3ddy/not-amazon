# Threat Checklist (Story/PR)

## Identity / Access
- [ ] Authentication enforced where required
- [ ] Authorization checked server-side
- [ ] Role escalation prevented

## Input / Output
- [ ] Input validation present
- [ ] Injection risks reviewed (SQL/NoSQL/command/template)
- [ ] Output encoding/escaping reviewed

## Data Protection
- [ ] Sensitive data minimized
- [ ] Secrets not logged/exposed
- [ ] PII handling reviewed (if applicable)

## Abuse / Reliability
- [ ] Rate limiting / throttling considered
- [ ] Error messages non-leaky
- [ ] Auditability/logging sufficient
