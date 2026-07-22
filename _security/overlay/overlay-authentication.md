---
api_key_in: []
api_specs:
- filename: overlay-openapi.yml
  format: yaml
  label: Overlay Market Data API
  slug: overlay-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overlay/refs/heads/main/openapi/overlay-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Overlay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overlay secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Overlay
provider_slug: overlay
scheme_count: 1
schemes:
- description: No API key, token, or OAuth. All market-data endpoints are open.
  name: public
  sources:
  - openapi/overlay-openapi.yml
  type: none
slug: overlay-authentication
source_filename: overlay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.overlay.market/api/aggregator-market-data\nsummary:\n  types: [none]\n  detail: >-\n    The Overlay public market-data API requires no authentication — the docs\n    state the endpoints are public. Trading actions are authorized on-chain by\n    the wallet signing BSC transactions (chain id 56), not by an API credential.\nschemes:\n  - name: public\n    type: none\n    description: No API key, token, or OAuth. All market-data endpoints are open.\n    sources: [openapi/overlay-openapi.yml]\nonchain_authorization:\n  detail: >-\n    build/unwind transactions are signed by the trader's wallet and executed\n    against the Shiva trading contract (0xeB497c228F130BD91E7F13f81c312243961d894A)\n    on BSC. The published agent skill recommends a smart-contract account with\n    restricted permissions (Safe + Zodiac Roles) rather than a raw private key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overlay/refs/heads/main/authentication/overlay-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Defi
- DeFi
- Perpetual Futures
- Derivatives
- Trading
- Market Data
- BNB Smart Chain
- Blockchain
- Web3
---
