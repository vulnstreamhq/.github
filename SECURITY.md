# Security policy

Vulnstream processes untrusted vulnerability records and delivers data to
customer-controlled destinations. Source documents, filters, URLs, payloads,
credentials, and delivery responses must therefore be treated as untrusted
input.

Status: private alpha. Vulnstream does not yet operate a public security
response service or publish a response-time commitment.

## Reporting a vulnerability

Do not open a public issue for a suspected vulnerability, exposed credential,
private exploit detail, customer-data concern, or sensitive package inventory.

Use private vulnerability reporting on the affected repository when GitHub
shows that option. If no private reporting route is available, contact the
organization owner through the private channel used to arrange access and
identify only the affected project until a safe exchange is established.

Include:

- the affected component and tested version or commit;
- the impact and minimum conditions required to reproduce it;
- safe reproduction steps using synthetic data;
- relevant non-sensitive logs or request identifiers; and
- any temporary mitigation already applied.

Do not include API keys, webhook signing secrets, authorization headers,
customer payloads, proprietary package inventories, unrelated personal data,
or third-party credentials.

## Authorized testing

Test only systems, accounts, workspaces, and webhook destinations you own or
have explicit permission to assess. Do not degrade service for another user,
bypass workspace boundaries, or use live exploit payloads when a synthetic
proof is sufficient.

## Current response boundary

Only the current private-alpha source is maintained. Vulnstream has no public
security-support lifecycle, severity matrix, acknowledgement target,
remediation deadline, bug-bounty program, or counsel-reviewed safe harbor.

A hosted launch requires a monitored security address, a published encryption
option, supported-version policy, response targets, coordinated-disclosure
timeline, incident process, and reviewed safe-harbor language.
