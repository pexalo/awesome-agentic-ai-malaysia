# Awesome Agentic AI Malaysia: integrations

## Public capability status

This draft does not claim that any named third-party product, interface version, read/write scope, or region is currently supported. The categories below are evaluation patterns. Before publishing a specific integration claim, add a dated support matrix reviewed by the product owner, or link to the current authoritative product page.

## Integration categories

### 1. GitHub Issues for nominations, corrections, and disputes

Confirm the system owner, supported interface, authentication method, minimum scopes, data fields, rate limits, error contract, test environment, audit events, and support responsibility.

### 2. Pull requests for transparent editorial review

Confirm the system owner, supported interface, authentication method, minimum scopes, data fields, rate limits, error contract, test environment, audit events, and support responsibility.

### 3. GitHub Actions for Markdown linting and link checking

Confirm the system owner, supported interface, authentication method, minimum scopes, data fields, rate limits, error contract, test environment, audit events, and support responsibility.

### 4. Dependabot or equivalent monitoring for any supporting code

Confirm the system owner, supported interface, authentication method, minimum scopes, data fields, rate limits, error contract, test environment, audit events, and support responsibility.

### 5. Optional GitHub Pages output for accessible browsing

Confirm the system owner, supported interface, authentication method, minimum scopes, data fields, rate limits, error contract, test environment, audit events, and support responsibility.

## Preferred connection pattern

1. A validated business event creates a traceable task.
2. The integration layer authenticates with a dedicated, least-privilege identity.
3. Inputs are schema-checked and untrusted content is isolated.
4. Read operations retrieve only the data needed for the task.
5. Proposed write actions are validated, deduplicated, and approved where required.
6. The destination response is checked before task state is updated.
7. Logs, metrics, and exception records are emitted without unnecessary sensitive content.

## Readiness checklist

- [ ] Named business and technical owners
- [ ] Approved interface and documented version
- [ ] Sandbox or safe test path
- [ ] Data classification and field-level minimisation
- [ ] Authentication, scopes, rotation, and revocation
- [ ] Rate limits, timeouts, retries, and idempotency
- [ ] Validation for inputs, outputs, and write actions
- [ ] Approval and separation-of-duties rules
- [ ] Audit events, alerts, exception queue, and reconciliation
- [ ] Retention, deletion, backup, recovery, and offboarding
- [ ] Vendor terms, privacy, security, and support review

## Integration record template

| Field | Required detail |
|---|---|
| System and owner | Name, business owner, technical contact |
| Purpose | The exact workflow need and expected outcome |
| Interface | API, webhook, event, file, database view, or other approved method |
| Identity | Service identity, authentication, scopes, and rotation |
| Data | Fields read or written, classification, retention, residency |
| Actions | Allowed operations, validation, approval, and limits |
| Reliability | Rate limit, timeout, retry, idempotency, and fallback |
| Evidence | Logs, audit events, reconciliation, and success measures |
| Exit | Disable, revoke, export, delete, and manual-continuity plan |

See [Pexalo integrations](https://pexalo.com/integrations) for the current public overview. Confirm actual availability and scope before making an implementation decision.
