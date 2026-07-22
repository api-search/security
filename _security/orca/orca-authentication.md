---
api_key_in: []
api_specs:
- filename: orca-openapi-original.json
  format: json
  label: Orca Public API
  slug: orca-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orca/refs/heads/main/openapi/orca-openapi-original.json
auth_types:
- none
description: 'Authentication posture for the Orca Public REST API. The API is deliberately open: "The Orca Public API is open and does not require authentication for read access." There are no OpenAPI securitySchemes. Write access to the protocol is not via this API — it happens on-chain by signing Solana transactions with the user''s own wallet keypair (client-side, via the SDKs).'
kind: authentication
layout: security
method: searched
name: Orca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orca secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orca
provider_slug: orca
scheme_count: 0
schemes: []
slug: orca-authentication
source_filename: orca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.orca.so/api-reference/overview\ndescription: >-\n  Authentication posture for the Orca Public REST API. The API is deliberately\n  open: \"The Orca Public API is open and does not require authentication for read\n  access.\" There are no OpenAPI securitySchemes. Write access to the protocol is\n  not via this API — it happens on-chain by signing Solana transactions with the\n  user's own wallet keypair (client-side, via the SDKs).\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\nschemes: []\nonchain_authorization:\n  model: wallet-signature\n  detail: >-\n    State changes (swaps, opening/closing positions) are Solana transactions\n    signed locally by the wallet keypair; there is no server-side API credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orca/refs/heads/main/authentication/orca-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Defi Dex
- DeFi
- DEX
- Solana
- AMM
- Liquidity
- Concentrated Liquidity
- Blockchain
- Crypto
---
