---
api_key_in: []
api_specs:
- filename: valora-api-openapi.yml
  format: yaml
  label: Valora API
  slug: valora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valora/refs/heads/main/openapi/valora-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: derived
name: Valora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valora secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Valora
provider_slug: valora
scheme_count: 0
schemes: []
slug: valora-authentication
source_filename: valora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/valora-api-openapi.yml + https://github.com/divvi-xyz/hooks (src/api/index.ts) + live probes (2026-07-21)\nnotes: >-\n  The Valora API is public and requires no authentication: the open-source\n  hooks-api declares no security schemes, enables CORS with origin '*', and\n  all endpoints answered live probes without credentials. Security derives\n  from the flow design — mutating operations (getSwapQuote, triggerShortcut,\n  simulateTransactions) only return unsigned transactions that must be signed\n  client-side by the wallet holder's key, so possession of the private key is\n  the effective authorization boundary. The wallet app itself is\n  self-custodial (keys never leave the device).\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\nschemes: []\nclient_side_signing:\n  required_for: [getSwapQuote, triggerShortcut, simulateTransactions]\n  details: Unsigned EVM transactions are returned to the client;\
  \ signing happens in the wallet with the user's key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valora/refs/heads/main/authentication/valora-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Cryptocurrency
- Wallet
- Payments
- DeFi
- Blockchain
- Celo
- Mobile
---
