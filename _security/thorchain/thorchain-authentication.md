---
api_key_in: []
api_specs:
- filename: thorchain-thornode-openapi.yaml
  format: yaml
  label: THORNode API
  slug: thornode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thorchain/refs/heads/main/openapi/thorchain-thornode-openapi.yaml
- filename: thorchain-midgard-openapi.json
  format: json
  label: Midgard API
  slug: midgard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thorchain/refs/heads/main/openapi/thorchain-midgard-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Thorchain Authentication
name_suffix: Authentication
oauth_flows: []
overview: THORChain declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: THORChain
provider_slug: thorchain
scheme_count: 0
schemes: []
slug: thorchain-authentication
source_filename: thorchain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/thorchain-thornode-openapi.yaml, openapi/thorchain-midgard-openapi.json\ndocs: https://dev.thorchain.org/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  access: open\n  note: >-\n    Both THORChain public APIs — the THORNode REST API and the Midgard indexer\n    API — are open, read-only, and require NO authentication. Neither OpenAPI\n    declares any securityScheme; there are no API keys, OAuth flows, or bearer\n    tokens. Access is unauthenticated GET over HTTPS. Public gateways (e.g.\n    Liquify, Nine Realms) may apply per-IP rate limiting, and some third-party\n    hosted endpoints offer optional API keys for higher rate tiers, but the\n    protocol APIs themselves define no auth. Write access to THORChain happens\n    on-chain: state changes are effected by broadcasting signed L1 transactions\n    with encoded memos to inbound vault addresses, not by calling an authed API.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thorchain/refs/heads/main/authentication/thorchain-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Crypto Web3
- Blockchain
- DeFi
- Cross-chain
- Liquidity
- Decentralized Exchange
- Cosmos
- Web3 Infrastructure
---
