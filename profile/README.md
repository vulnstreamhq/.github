<p align="center">
  <img src="../assets/vulnstream-mark.svg" width="112" alt="Vulnstream">
</p>

# Vulnstream

**Dependable change-data infrastructure for vulnerability intelligence.**

Vulnstream turns upstream vulnerability records into normalized semantic events with immutable provenance, durable replay, and verifiable delivery. It is infrastructure with an explorer—not an explorer with webhooks added around it.

## What we are building

- Stable, typed changes instead of order-sensitive vulnerability JSON diffs.
- A traceable chain from exact source input to normalized version and event identity.
- Replay that supports recovery, backfills, and integration testing without depending on broker retention.
- At-least-once delivery with deterministic IDs, signed payloads, retries, and attempt evidence.
- An explorer that makes those contracts inspectable without becoming the system of record.

## Current stage

Vulnstream is in private alpha. The event, provenance, reconstruction, replay, outbox, subscription, and signed-webhook foundations run locally. Hosted environments, managed identity, commercial billing, and service-level commitments are not yet available.

The product repository remains private while licensing, history, security, and commercial-launch decisions are completed. Public claims will follow measured behavior, not roadmap intent.

## Trust principles

1. Event quality before source count.
2. Provenance is part of every contract.
3. PostgreSQL owns replay and recovery; the broker is transport.
4. At-least-once semantics are explicit and deduplicable.
5. Delivery is not complete until its outcome is visible.

For security-sensitive matters, follow the affected repository's security policy and never publish credentials, private exploit details, customer data, or package inventories in a public issue.
