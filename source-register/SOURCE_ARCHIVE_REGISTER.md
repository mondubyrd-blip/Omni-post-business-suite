# Source Archive Register

All hashes below are SHA-256 values computed from the uploaded ZIP bytes during this review. Original archives were not modified.

| Uploaded archive | Bytes | SHA-256 | Review classification |
|---|---:|---|---|
| `Copy of OmniPulse_Business_Suite_v1.0_FIXED_PROD.zip` | 71,389 | `1d10fa4f961d8c0f15e022fd40565906e3e87fddc7286d43e809beac620ab3b4` | OmniPulse source package |
| `OmniPulse_Business_Suite_v1.0_PROD(1).zip` | 71,389 | `1d10fa4f961d8c0f15e022fd40565906e3e87fddc7286d43e809beac620ab3b4` | Byte-identical duplicate of preceding archive |
| `Reusable_Turnkey_Business_Template.zip` | 25,594 | `8b4b56af6f9d87f1eb3dcb49f7f089bd4f71a818b768c305f47ccb4421454e67` | Reusable store clone template |
| `Empower_Express_Omnipresence_Hub_v1.0.zip` | 89,716 | `a82fad8bbc13806c9e80d9089f55bc1767b024e0c3cf27d6715c3de3f5eac064` | AutoLister / omnipresence retail application |
| `Empower_Express_Drop_Chat_Standalone.zip` | 5,339 | `6655c466125878253ecfde9a4ff9a8e4ce585b28cd3bf947a9e5e0e27ab8449e` | Standalone one-file chat page |
| `Empower_Express_Enterprise_Master_Suite_Final(1).zip` | 289,701 | `2aeb6cc0832948ec3f0573f6f3d4fcfaa4bc3c91d6d5518c1bfdbc966e21b4f5` | Retail master package with duplicated app trees and operations documents |
| `Empire_Express_Deal_Master_Dossier_SHA256.zip` | 372,181 | `18199f36980dce82d1109ee41ce42ed5c39d3e5de7b274392673a7275ba4d1ec` | Dossier containing nested Empower/Empire retail, Lily, and reusable-template archives |
| `ShangTemple_Agape_Senior_Voice_Companion_DEV.zip` | 579 | `aba802b0714941180bcc58bbe1082abb0d5d84a7294973ddf684a990f674f810` | Two-document AGAPE architecture/planning archive; no implementation source |
| `ShangTemple_PWA_Suite_Deployable.zip` | 21,002 | `6a7b7ede7eb04cc4bb8020b56fba4431a5675015d3e6b393d320ad79313de35d` | Five unrelated PWA examples |
| `ION_Custom_Avatar_Business_Plan_Pack(1).zip` | 147,827 | `686f0c4c8f42dd29f2a1f483edec1991b2d6eab704be43520ffd5a534ecca3f0` | Separate avatar-production business pack; excluded from thrift-store integration |

## Duplicate and packaging findings

- The two top-level OmniPulse ZIPs are byte-identical: same 71,389-byte size and SHA-256.
- The Empire Express Deal Master Dossier contains nested ZIPs for:
  - Empower Express Storefront and Omnipresence Suite.
  - Lily's Thrift Store Community Branch.
  - Reusable Business Clone Template.
- The Enterprise Master Suite contains repeated software-engine directory trees and overlapping AutoLister/Omnipresence components. These are candidates for source comparison, not separate products to merge blindly.
- The standalone Drop Chat archive contains only `index.html`.
- The AGAPE DEV archive contains only `README.txt` and `ARCHITECTURE.txt`; it is not a working engine package.

## GitHub staging note

This register and the integration documents are committed to this repository. The original ZIP binaries are not yet stored in GitHub; the source archives remain preserved in the user's uploaded workspace. Do not treat a filename or this hash register as proof that a ZIP has been committed.
