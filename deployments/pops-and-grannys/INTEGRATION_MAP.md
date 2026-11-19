# Pops & Granny's Integration Map

## Product identity
- Customer-facing business: **Pops & Granny's Thrift Store**
- Business platform: **OmniPulse Business Suite**
- Deployment type: separate tenant / branded deployment.
- Location reference supplied by the owner: off Wilcox, Chattanooga, Tennessee. Exact street address, contact details, hours, and domain remain unconfigured.

OmniPulse is the reusable suite name, not the store's brand.

## Recommended composition

| Layer | Source application/component | Use in deployment | Boundary |
|---|---|---|---|
| Business operations shell | OmniPulse Business Suite | Dashboard, inventory/sales overview, promotions, calendar, domains, reports | Keep generic suite branding separate from store branding |
| Store configuration | Reusable Turnkey Business Template | Store-specific setup, storefront, operations pages, plugin config | New store ID and config; no inherited example data |
| Storefront | Turnkey universal storefront + current Pops & Granny's PWA starter | Product browsing, store information, pickup requests | Store-specific products and policies |
| Item intake / listing | Empower Express Omnipresence Hub / AutoLister AI | Photo intake, item attributes, pricing research, listing drafts | AI provider and credentials require explicit configuration |
| Consignment | Consignor Split Widget / ledger / agreements | Vendor onboarding, split calculation, payout reporting | Enable only if this store uses consignors; ratios must be set by owner |
| Omnichannel publishing | OmniPulse post composer + Empower marketplace selector | Prepare channel-specific listings and promotional posts | Draft-first; no live posting until account authorization and channel APIs are verified |
| Customer drop chat | Empower Express Drop Chat | Customer questions and new-drop announcements | Review data flow, storage, and external dependencies first |
| Senior experience | Lily suite UX patterns | Large controls, clear navigation, accessible task flows | Do not import Lily's nonprofit/client eligibility rules |
| Voice assistance | Lily's Agape Immediate Presence concept + AGAPE Companion architecture | Voice navigation, spoken help, intent routing, knowledge lookup, TTS | Actual AGAPE implementation is not present in the DEV archive; browser speech is not equivalent |
| PWA/offline | Existing PWA shell patterns + Pops & Granny's PWA starter | Install prompt, manifest, service worker, offline app shell | Confirm offline data writes, sync conflicts, and update behavior |

## Suggested navigation

1. Home
2. Browse Store
3. New Arrivals / Drop Feed
4. Ask AGAPE (voice and text assistance)
5. Inventory (staff)
6. Add Item (staff photo intake)
7. Sales / Checkout (staff)
8. Vendors & Payouts (only if consignment is enabled)
9. Promotions & Social Posts
10. Reports
11. Accessibility & Voice Settings

## Data model boundaries

Use a store/tenant identifier on all store-owned records:
- Store profile and operating configuration.
- Products, photos, category, condition, price, status, and stock.
- Sales, refunds, and tender references.
- Customer contact/consent records.
- Vendor/consignor records and payout ledger (if enabled).
- Promotions and publication drafts.
- AGAPE preferences and local knowledge packs.

Do not copy customer or volunteer records from Lily's. Do not reuse Lily's client ID or eligibility ledger. Do not reuse Empower Express sample inventory, vendor records, or financial figures as Pops & Granny's real data.

## Integration order

### Phase A — establish tenant boundary
Create a unique store ID, store configuration, branding, hours, address, currency, tax settings, inventory policy, returns policy, and domain. Keep all sample/demo records clearly marked.

### Phase B — retail core
Connect storefront, product catalog, inventory, and checkout to one canonical data model. Define stock movement and transaction audit behavior before enabling sales.

### Phase C — resale operations
Add camera intake, AI attribute suggestions, price research, listing drafts, and vendor split ledger only after confirming whether the store is owner-stocked, consignment-based, or mixed.

### Phase D — OmniPulse operations
Connect promotions, calendar, local marketplace drafts, and performance reporting. External publishing remains approval-gated.

### Phase E — senior accessibility and AGAPE
Implement accessible text sizing, contrast, keyboard/touch navigation, spoken prompts, speech input/output, and local help retrieval. Integrate a real AGAPE engine only after its implementation and runtime contract are available.

### Phase F — PWA hardening
Validate installability, HTTPS deployment, service-worker caching, offline reads, safe local writes, reconnection, conflict handling, and update behavior on Android and desktop.

## Explicit exclusions
- Lily's nonprofit client distribution rules, volunteer administration, workforce intake, community kitchen, and meal/shelter accounting.
- ION avatar-production business assets.
- NetNavi, Sentinel, YubiKey Vault, AquaLine, and MediaIntel product functionality from the unrelated PWA collection.
- Unverified live marketplace automation, payment processing, or vendor payouts.

## Open implementation facts (not yet established)
- Exact Wilcox street address, store phone, hours, and domain.
- Store ownership model: owned inventory, consignment, or mixed.
- Tax and return policies.
- POS/payment provider.
- Whether customer chat requires accounts or is anonymous.
- Actual AGAPE runtime source, speech provider, local model/voice availability, and offline support.
- Whether OmniPulse's Gemini-backed features are permitted for this deployment or require local/offline substitutes.
