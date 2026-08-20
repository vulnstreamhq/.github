# Contributing

Vulnstream repositories define their own setup, validation, review, and release
requirements. Read the affected repository's `README.md`, contribution guide,
and security policy before opening an issue or pull request. Repository-specific
instructions take precedence over this organization-wide default.

The core product repository is currently private. Access does not imply that a
repository accepts unsolicited contributions or grants permission to
redistribute its code.

## Product boundary

Changes must preserve Vulnstream's position:

> Dependable change-data infrastructure for vulnerability intelligence:
> normalized semantic events, immutable provenance, replay, and verifiable
> delivery.

The explorer, documentation, and destinations should explain, inspect, or
consume those contracts rather than create a competing source of truth.

Before proposing a material capability, identify:

1. which product guarantee it strengthens;
2. which source, event, replay, filter, or delivery contract it changes;
3. how retries, ordering, idempotency, and partial failure behave;
4. what durable evidence will prove the capability works; and
5. which documentation, schema, migration, security, and operational surfaces
   must change with it.

## Submission expectations

- Use synthetic or public fixtures. Do not commit customer data, credentials,
  private package inventories, or production identifiers.
- Keep source-native facts and attribution intact; do not silently collapse
  disagreements between vulnerability sources.
- Add automated tests for contract behavior and failure boundaries.
- Update public documentation when behavior, status, setup, or compatibility
  changes.
- Follow the affected repository's formatting, lint, test, commit-signing, and
  review requirements.
- Route sensitive findings through the [security policy](./SECURITY.md), not a
  public issue or pull request.
