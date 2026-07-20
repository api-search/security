---
api_key_in: []
api_specs:
- filename: kamino-public-openapi-original.json
  format: json
  label: Kamino Public API
  slug: kamino-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kamino/refs/heads/main/openapi/kamino-public-openapi-original.json
- filename: kamino-transactions-openapi-original.json
  format: json
  label: Kamino Transactions API
  slug: kamino-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kamino/refs/heads/main/openapi/kamino-transactions-openapi-original.json
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Kamino Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kamino secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kamino
provider_slug: kamino
scheme_count: 0
schemes: []
slug: kamino-authentication
source_filename: kamino-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.kamino.finance/openapi/json ; https://kamino.com/build/api-reference/introduction\ndocs: https://kamino.com/build/api-reference/introduction\nsummary:\n  types:\n  - none\n  api_key_in: []\n  oauth2_flows: []\nnote: 'The Kamino Public API declares no securitySchemes in its OpenAPI: read/data\n  and unsigned-transaction-building endpoints are open. Requests are RATE-LIMITED\n  for unauthenticated users; API keys for higher limits are granted on request. A\n  small number of routes return 401 when elevated access is required. Transactions\n  are returned UNSIGNED and must be signed client-side with the user''s Solana wallet\n  — Kamino never holds keys.'\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kamino/refs/heads/main/authentication/kamino-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Crypto Web3
- DeFi
- Solana
- Lending
- Borrowing
- Yield
- Blockchain
- Oracle
- Vaults
---
