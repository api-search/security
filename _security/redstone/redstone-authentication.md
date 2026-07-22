---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Redstone Authentication
name_suffix: Authentication
oauth_flows: []
overview: RedStone secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RedStone
provider_slug: redstone
scheme_count: 1
schemes:
- description: The RedStone cache/price API and oracle gateway are public and read-only; no API key, token, or OAuth is required to fetch signed data packages or historical prices.
  name: public-read
  sources:
  - https://api.redstone.finance
  - https://oracle-gateway-1.a.redstone.finance
  type: none
slug: redstone-authentication
source_filename: redstone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.redstone.finance/docs/introduction\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: public-read\n  type: none\n  description: >-\n    The RedStone cache/price API and oracle gateway are public and read-only; no API key, token,\n    or OAuth is required to fetch signed data packages or historical prices.\n  sources: [https://api.redstone.finance, https://oracle-gateway-1.a.redstone.finance]\ndata_integrity:\n  model: signed-data-packages\n  description: >-\n    Trust is enforced cryptographically rather than by API authentication. Every data package is\n    signed with the provider's ECDSA key; responses include liteEvmSignature and providerPublicKey\n    so consumers verify authenticity on-chain (via the EVM/chain connectors) or off-chain.\nnotes: >-\n  Push-model contract deployment and relayer operation use the RedStone CLI and on-chain accounts;\n  those are chain-level credentials,\
  \ not an HTTP API auth scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redstone/refs/heads/main/authentication/redstone-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Infrastructure
- Blockchain
- Oracle
- DeFi
- Price Feeds
- Data
- Web3
- Smart Contracts
---
