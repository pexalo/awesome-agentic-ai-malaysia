# Awesome Agentic AI Malaysia: security and governance

## Scope

This page records public design principles and a review checklist. It is not a warranty, audit report, certification, data-processing agreement, threat model for a specific deployment, or substitute for qualified legal and security review.

## Priority practices

- Review every destination before merging; avoid URL shorteners and unexplained downloads.
- Pin or restrict automated workflow permissions and review third-party actions.
- Never place tokens, personal data, or confidential reports in issues or pull requests.
- Use a private disclosure channel for malicious links or repository vulnerabilities.
- Preserve disclosure of contributor affiliations and potential conflicts of interest.

## Threats to consider

- Unauthorised access, over-broad permissions, or credential exposure
- Prompt injection, malicious documents, unsafe URLs, and untrusted tool output
- Sensitive-data disclosure through prompts, logs, caches, analytics, or generated output
- Incorrect, duplicated, irreversible, or out-of-order write actions
- Dependency compromise, vulnerable packages, insecure workflow actions, or model-provider changes
- Hallucinated facts, invalid structured output, biased classification, or unsupported decisions
- Cross-client, cross-role, or cross-environment data leakage
- Service failure, runaway retries, uncontrolled cost, or missing incident escalation
- Rights, consent, retention, and regulatory failures

## Control framework

### Before build

1. Name the business owner, technical owner, security owner, and incident contacts.
2. Classify data and map every authorised source and destination.
3. Define prohibited uses, approval points, access scopes, retention, and deletion.
4. Document task-specific acceptance, safety, and stop criteria.
5. Complete vendor, dependency, privacy, and threat review appropriate to risk.

### Before launch

1. Test representative and adversarial inputs, permission denial, timeouts, duplicates, and partial failure.
2. Verify secrets storage, key rotation, environment separation, and least privilege.
3. Confirm audit events, alerts, exception queues, rollback, and manual fallback.
4. Review user notices, consent, terms, accessibility, and record-keeping needs.
5. Obtain formal approval from the named owners.

### During operation

1. Monitor outcome quality, corrections, incidents, drift, cost, latency, and access.
2. Review permissions and retained data on a defined schedule.
3. Re-test after material changes to models, prompts, data, tools, or policy.
4. Pause or restrict the workflow when safety or reliability thresholds are breached.
5. Record incidents and corrective actions, then update tests to prevent recurrence.

## Public repository hygiene

- Never commit secrets, private endpoints, customer identifiers, personal data, or confidential screenshots.
- Use synthetic examples and clearly marked placeholders.
- Restrict CI permissions, pin third-party actions, scan changes, and review generated files.
- Provide a private route for responsible disclosure before enabling public contributions.

For Pexalo's current public security positioning, see [Security & governance](https://pexalo.com/security). Deployment-specific commitments belong in the relevant agreement.
