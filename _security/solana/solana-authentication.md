---
api_key_in: []
api_specs:
- filename: solana-rpc-api-openapi.yml
  format: yaml
  label: Solana RPC Accounts API
  slug: solana-rpc-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/openapi/solana-rpc-api-openapi.yml
auth_types: []
description: The Solana JSON-RPC OpenAPI declares no securitySchemes. The public cluster endpoints (api.mainnet-beta.solana.com, api.devnet.solana.com, api.testnet.solana.com) require no API key and no authentication — they are open, shared, rate-limited infrastructure not intended for production. Authenticated access is provided by third-party RPC providers (Helius, QuickNode, Triton, Alchemy, Syndica, GetBlock, etc.), which typically authenticate via an API key embedded in the request URL path/query or a header. Those keys are provider-specific and not part of the Solana protocol.
kind: authentication
layout: security
method: searched
name: Solana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solana declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Solana
provider_slug: solana
scheme_count: 0
schemes: []
slug: solana-authentication
source_filename: solana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/solana-rpc-api-openapi.yml\ndocs: https://solana.com/docs/rpc\ndescription: >-\n  The Solana JSON-RPC OpenAPI declares no securitySchemes. The public cluster endpoints\n  (api.mainnet-beta.solana.com, api.devnet.solana.com, api.testnet.solana.com) require no API\n  key and no authentication — they are open, shared, rate-limited infrastructure not intended\n  for production. Authenticated access is provided by third-party RPC providers (Helius,\n  QuickNode, Triton, Alchemy, Syndica, GetBlock, etc.), which typically authenticate via an\n  API key embedded in the request URL path/query or a header. Those keys are provider-specific\n  and not part of the Solana protocol.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_endpoints_unauthenticated: true\nschemes: []\nnotes:\n  - Public RPC: no credentials; may return HTTP 429 (rate limited) / 403 (blocked).\n  - Private RPC providers: bearer/API-key\
  \ auth, out of scope for the core protocol.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/authentication/solana-authentication.yml
summary_line: 0 schemes
tags:
- Blockchain
- Cryptocurrency
- Web3
- DeFi
- Transactions
- Tokens
---
