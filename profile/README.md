# Vulnstream

<img src="../assets/vulnstream-logo.png" width="176" alt="Vulnstream logo">

**Dependable change-data infrastructure for vulnerability intelligence.**

Vulnstream continuously observes vulnerability sources, retains exactly what
they published, normalizes meaningful changes, reconciles missed updates, and
proves what was delivered to downstream systems.

Vulnstream is a vulnerability-event infrastructure product with an explorer,
not an explorer product with webhooks added around it.

## The product contract

```text
Source revision → Raw evidence → Normalized version → Semantic event → Replay → Delivery evidence
```

| Guarantee | What it means |
| --- | --- |
| Normalized semantic events | Stable, typed changes represent material vulnerability updates instead of arbitrary JSON churn. |
| Immutable provenance | Source revisions, exact raw records, hashes, observation times, and normalized versions remain connected. |
| Deterministic replay | Consumers recover from a durable system of record without depending on broker retention. |
| Verifiable delivery | Deterministic IDs, signed payloads, retries, and attempt records make at-least-once delivery inspectable. |

## Who Vulnstream is for

Vulnstream is built for application-security, vulnerability-management, and
security-platform teams that maintain automated workflows around public
vulnerability intelligence. It is intended to replace bespoke polling,
comparison ledgers, reconciliation jobs, and delivery plumbing—not scanners,
asset inventories, ticketing systems, or security judgment.

## What exists today

The private-alpha foundation runs locally and includes:

- a CVE List V5 production-candidate connector with immutable Git checkpoints,
  incremental observation, daily reconciliation, quarantine, and exact raw
  artifact preservation;
- normalized CVE versions and deterministic CloudEvents for publication,
  modification, lifecycle, CVSS, affected-product, reference, CISA KEV, and
  package URL changes;
- transactional PostgreSQL writes for immutable versions, events, and a durable
  outbox, with Kafka-compatible publication as replaceable transport;
- observed and reconstructed replay with explicit provenance, effective and
  observation time, and query-bound cursors;
- shared filters, workspace-scoped API keys, subscriptions, signed webhook
  delivery, retries, and retained attempt evidence; and
- a browser explorer that inspects records, source material, semantic changes,
  and integration contracts without becoming the system of record.

One complete local historical run processed 70,638 upstream commits into
814,571 material versions and 1,046,499 reconstructed semantic events. Those
figures are local capacity evidence, not a hosted service-level result.

## Current stage

Vulnstream is a private alpha. There is no public hosted service, managed
customer identity, checkout flow, support service-level agreement, or
production availability commitment.

The immediate milestone is a managed CVE List V5 source proof: continuous
staging operation, failure injection, missed-update reconciliation, recovery
drills, and measured source-to-event freshness. The milestone concludes with a
traceable source-to-webhook demonstration backed by retained raw, event,
replay, and delivery evidence.

## Project visibility

The core product repository remains private while licensing, history, security,
and commercial-launch decisions are completed. This public `.github`
repository intentionally contains only the organization profile and shared
community-health guidance. Public claims describe measured or locally
executable behavior and distinguish it from planned hosting.

## Trust and participation

- Review the organization-wide [security policy](../SECURITY.md) before
  reporting sensitive behavior.
- Use [support guidance](../SUPPORT.md) for non-sensitive questions and product
  feedback.
- Read [contribution expectations](../CONTRIBUTING.md) before proposing a
  change in a repository that accepts contributions.
- Follow the [code of conduct](../CODE_OF_CONDUCT.md) in every Vulnstream
  project space.

Do not publish credentials, private exploit details, customer data, package
inventories, or sensitive infrastructure information in a public issue.
