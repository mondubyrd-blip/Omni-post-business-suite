# Application Inventory (source-derived)

Scope: uploaded business-related archives in the current workspace. This is an inventory of what the files actually contain, not a claim that every feature has passed runtime testing.

## 1. OmniPulse Business Suite — reusable platform
**Source:** `Copy of OmniPulse_Business_Suite_v1.0_FIXED_PROD.zip` and `OmniPulse_Business_Suite_v1.0_PROD(1).zip`

The two uploaded archives have identical SHA-256 hashes and identical 31-entry layouts; treat them as duplicate copies, not separate products.

**Documented modules**
- Executive dashboard and reporting.
- AI post composer and timing scheduler for social channels.
- Promotions and calendar hub with .ics export.
- Inventory and sales manager.
- Domain, DNS, redirect, and microsite management.
- Local marketplace/classified listing hub and selling-place index.
- Maker-Operator operating system: air-gap handoff, interruption shield, weekly sync, operator SLA, and authority arbitration.

**Role in Pops & Granny's:** platform shell / management layer. It should host or link retail modules, not replace their specialized workflows.

**Implementation note:** metadata and package files declare a React 19 + TypeScript + Vite/Express app with a server-side Gemini integration capability. Verify configuration and secrets handling before enabling AI services.

## 2. Reusable Turnkey Business Template — store cloning foundation
**Source:** `Reusable_Turnkey_Business_Template.zip`; duplicate copy is also embedded in the Empire Express Deal Master Dossier.

**Files:** `universal_storefront.html`, `universal_operations_suite.html`, `setup_wizard.html`, `store_config.json`, commercial license binding, dependency watchdog, and barcode / POS hardware / SMS-drop extensions.

**Role in Pops & Granny's:** tenant/store configuration, storefront baseline, operations baseline, and optional hardware/notification extensions. Configure a separate store ID, name, domain, address, policy, and plugins. Do not copy the example store identity or example business policies as facts.

## 3. Empower Express Omnipresence Hub / AutoLister AI — resale intake and listing
**Source:** `Empower_Express_Omnipresence_Hub_v1.0.zip`; also represented in the Enterprise Master Suite and Empire Express Deal Master Dossier.

**Documented workflow**
- Camera/photo intake.
- Gemini multimodal item identification (brand, category, material, color, condition).
- Price comparisons and listing draft.
- Configurable consignor split (documented examples: 50/50, 60/40, 70/30).
- Inventory aging and vendor payout dashboard.
- Multi-channel syndication to storefront, Facebook, Instagram, and Google Business Profile.

**Role in Pops & Granny's:** high-value retail module, subject to business model choice. Consignor splits and payout methods should be enabled only if Pops & Granny's actually accepts consigned inventory.

**Status caveat:** source README describes intended capabilities; live marketplace publishing and end-to-end payouts are not certified by this inventory.

## 4. Empower Express / Empire Express Enterprise Master Suite — retail operations package
**Source:** `Empower_Express_Enterprise_Master_Suite_Final(1).zip`

Contains a start-here operations portal, commercial license agreement, retail expansion playbook, vendor consignment agreement, hardware/network specification, local marketplace automation wizard, standalone live-drop chat page, and multiple copies of the AutoLister/Omnipresence React application tree.

**Role in Pops & Granny's:** source of retail operating procedures, drop chat, consignment forms, and possible hardware integrations. Multiple nested software-engine directories appear to be variants/copies; compare before selecting one canonical source.

## 5. Empower Express Drop Chat — customer communication component
**Source:** `Empower_Express_Drop_Chat_Standalone.zip` (one `index.html`).

**Role in Pops & Granny's:** candidate customer drop/availability chat surface. Inspect the HTML and its external dependencies before connecting it to store data. Not a separate business-management suite.

## 6. Lily's Thrift Store & Community Kitchen Operations Suite — senior/community reference
**Source:** `Lilys_Thrift_Store_Community_Branch.zip` nested inside `Empire_Express_Deal_Master_Dossier_SHA256.zip`.

**Documented modules**
- Client free clothing desk with eligibility / distribution rules.
- Supporter thrift drops and pickup reservations.
- Volunteer registration, shifts, check-in, and hour exports.
- Workforce intake / vocational training.
- Director hub and discretionary price control.
- Agape Immediate Presence voice engine. Inspection of the Lily suite HTML shows this is browser `speechSynthesis` / `SpeechSynthesisUtterance` output with a hard-coded informational message and alert; no browser speech-recognition API was found in that file. It is a basic TTS helper, not a full conversational speech engine.
- Local/offline browser and launcher paths.

**Role in Pops & Granny's:** reference for senior-friendly navigation, voice interaction, and accessible workflow design only. Keep Lily's community eligibility, donation-to-meal/shelter accounting, volunteer, and workforce policies isolated; they are not default commercial thrift-store rules.

## 7. AGAPE Senior Voice Companion — voice architecture reference
**Source:** `ShangTemple_Agape_Senior_Voice_Companion_DEV.zip`.

This archive contains only `README.txt` and `ARCHITECTURE.txt`. It specifies an offline-first Linux plan, local knowledge retrieval, voice-first interface, and the flow: Application → Intent Detection → Knowledge Search → Response → Text-to-Speech.

**Role in Pops & Granny's:** architectural reference / integration target. This archive is planning documentation, not a working speech-engine implementation.

## 8. ShangTemple PWA Suite — reusable PWA patterns
**Source:** `ShangTemple_PWA_Suite_Deployable.zip`.

Contains five PWAs: NetNavi Avatar, Sovereign Sentinel, YubiKey Vault, AquaLine Breeder, and MediaIntel Vision. These are not thrift-store business applications. Reuse only generic PWA patterns (manifest, service worker, installability, offline shell) after reviewing each implementation; do not bundle their product functionality into this retail app by default.

## 9. Empire Express Deal Master Dossier — packaging / provenance container
**Source:** `Empire_Express_Deal_Master_Dossier_SHA256.zip`.

Contains nested archives for the Empower/Empire retail suite, Lily's community branch, and reusable business clone template, plus a SHA256SUMS file and expanded retail documents. This is a packaging/provenance bundle, not another independent application.

## 10. ION Custom Avatar Business Plan Pack — not part of retail suite
**Source:** `ION_Custom_Avatar_Business_Plan_Pack(1).zip`.

Business plan, avatar production SOPs, capture checklists, legal drafts, provenance/budget templates, and runtime handoff notes. Exclude from Pops & Granny's integration; it is a separate avatar-production business package.
