# Vulnstream organization profile

This is the intentionally public GitHub organization-profile repository for
Vulnstream. GitHub renders [`profile/README.md`](./profile/README.md) on the
[`vulnstreamhq`](https://github.com/vulnstreamhq) organization overview.

The repository also provides default community-health files to Vulnstream
repositories that do not define a repository-specific version:

| File | Purpose |
| --- | --- |
| [`SECURITY.md`](./SECURITY.md) | Routes sensitive reports without exposing credentials or exploit details. |
| [`SUPPORT.md`](./SUPPORT.md) | Distinguishes support, product feedback, and security reports. |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md) | Establishes organization-wide contribution expectations. |
| [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md) | Defines professional participation and enforcement expectations. |

Repository-specific instructions override these defaults when they provide a
more precise setup, validation, security, or support process.

## Public-content boundary

Keep this repository public so GitHub can display the public organization
profile. Do not store private roadmaps, customer information, credentials,
security reports, internal architecture, package inventories, or production
configuration here. Member-only organization-profile content belongs in a
private `.github-private` repository if that surface is needed later.

Third-party source and product names may be used only to identify compatibility
or provenance. Do not add upstream logos, imply endorsement, or copy upstream
data into this repository. Keep required data-license notices with the product
outputs and documentation that actually reproduce the data.

## Updating the profile

Profile changes should update the approved brand asset and public copy in the
same review. Before merging:

1. Compare capability and maturity claims with the current product status and
   roadmap in the core repository.
2. Confirm that every public link resolves without requiring access to a
   private repository.
3. Check that images have meaningful alternative text and remain legible on
   light and dark GitHub themes.
4. Run Markdown lint and inspect the rendered organization overview.
5. Verify that no confidential or security-sensitive material is present.
6. Recheck source-data, dependency-license, and trademark notices whenever a
   new upstream source or named integration is introduced.
