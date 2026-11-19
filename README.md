# OmniPulse Business Suite — Multi-Business Workspace

This repository is the integration workspace for independently branded business deployments built on the reusable OmniPulse Business Suite and related turnkey retail components.

## Branding and product boundaries

- **OmniPulse Business Suite** is the reusable business platform / suite. It is not the storefront brand.
- **Pops & Granny's Thrift Store** is a distinct storefront deployment (Wilcox area, Chattanooga, Tennessee).
- **Lily's Thrift Store & Community Kitchen** is a separate community/nonprofit operations application and must remain unchanged.
- **Empower Express / Empire Express** source archives contain retail, consignment, omnichannel publishing, and expansion components. The uploaded archive labels predominantly say **Empower Express**; preserve that source naming until the business-facing name is confirmed.
- **Reusable Turnkey Business Template** supplies the configurable store clone, storefront, operations suite, and extension framework.

## Repository layout

- `catalog/` — source-derived application inventory and integration map.
- `source-register/` — archive provenance, hashes, duplicate detection, and component boundaries.
- `deployments/pops-and-grannys/` — deployment-specific configuration and integration plan.
- `applications/` — application source packages staged for integration.

## Integration direction

OmniPulse is the business-suite layer. Retail-specific applications contribute capabilities as modules:
1. Storefront and inventory.
2. Photo intake, AI-assisted item identification, and pricing comparisons.
3. Consignor/vendor split ledger and payout reporting.
4. Local marketplace listing and omnichannel publishing.
5. Drop chat / customer communications.
6. Senior-friendly user experience and AGAPE voice assistance.
7. Offline-capable PWA shell and local-first workflows.

Do not merge Lily's client eligibility, distribution limits, volunteer, workforce, or community-kitchen rules into a commercial thrift deployment. Reuse only explicitly appropriate components and preserve source licenses.

## Status

The initial repository commit contains the source-derived inventory and integration plan. Original uploaded ZIP archives have been inventoried locally; this commit does not claim that the original binary archives have been uploaded to GitHub. See `source-register/SOURCE_ARCHIVE_REGISTER.md`.
