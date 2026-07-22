---
api_key_in: []
auth_types:
- apiKey
- wallet-signature
description: ''
kind: authentication
layout: security
method: searched
name: Squads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Squads secures its APIs with apiKey and wallet-signature across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Squads
provider_slug: squads
scheme_count: 0
schemes: []
slug: squads-authentication
source_filename: squads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://grid.squads.xyz/\nnote: >-\n  Squads has two distinct developer surfaces with different auth models. No\n  in-repo OpenAPI was available to derive securitySchemes mechanically; this\n  profile is searched from the product docs.\nsummary:\n  types: [apiKey, wallet-signature]\nsurfaces:\n  - name: Grid API\n    kind: rest\n    auth: apiKey\n    detail: >-\n      Grid (stablecoin API for accounts, payments, cards, yield) authenticates\n      with an API key generated in the Grid dashboard (grid.squads.xyz).\n    docs: https://grid.squads.xyz/\n  - name: Squads Multisig\n    kind: onchain-sdk\n    auth: wallet-signature\n    detail: >-\n      The Multisig SDK (@sqds/multisig) and Rust crate build and sign Solana\n      transactions; authorization is enforced on-chain by the Squads Protocol\n      program (multisig member keys + thresholds), not by an API credential.\n    docs: https://docs.squads.so/main/development\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squads/refs/heads/main/authentication/squads-authentication.yml
summary_line: apiKey/wallet-signature · 0 schemes
tags:
- Company
- Infrastructure
- Blockchain
- Solana
- Multisig
- Smart Accounts
- Stablecoins
- Payments
- Wallet
- Web3
---
