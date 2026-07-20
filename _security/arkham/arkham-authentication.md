---
api_key_in:
- header
api_specs:
- filename: arkham-openapi-original.json
  format: json
  label: Arkham Intel API
  slug: arkham-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkham/refs/heads/main/openapi/arkham-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Arkham Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arkham secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arkham
provider_slug: arkham
scheme_count: 1
schemes:
- description: All API requests must include a valid API-Key header. Requests without it are rejected as unauthorized (401 "error validating API key"). Keys are created in the Arkham UI (Settings -> API Keys, or the API Dashboard) and shown once. Use the API-Key header, NOT Authorization.
  in: header
  name: ApiKeyHeader
  parameter: API-Key
  sources:
  - https://arkm.com/llms/guides/api-keys-authentication.md
  type: apiKey
slug: arkham-authentication
source_filename: arkham-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://arkm.com/llms/guides/api-keys-authentication.md\ndocs: https://arkm.com/llms/guides/api-keys-authentication.md\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The published OpenAPI (openapi/arkham-openapi-original.json) does not declare securitySchemes; the\n    auth model is documented in the API Keys & Authentication guide. All REST requests require an\n    API-Key header. The x402 agent surface (api.arkm.com/x402) uses payment (USDC on Base) or a\n    Sign-In-With-X wallet signature as its auth instead of an API key.\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: >-\n    All API requests must include a valid API-Key header. Requests without it are rejected as\n    unauthorized (401 \"error validating API key\"). Keys are created in the Arkham UI (Settings -> API\n    Keys, or the API Dashboard) and shown once. Use the\
  \ API-Key header, NOT Authorization.\n  sources:\n  - https://arkm.com/llms/guides/api-keys-authentication.md\nkey_management:\n  create: https://arkm.com/api-dashboard?tab=api-keys\n  settings: https://arkm.com/settings\n  default_key_limit: 5\n  rotation: create-new -> deploy -> revoke-old\n  best_practice: separate keys per environment (prod/staging/dev) and per service\nx402_auth:\n  base_url: https://api.arkm.com/x402\n  model: payment-is-auth\n  payment_protocol: x402 v2 (EIP-3009 USDC transfer authorization on Base, eip155:8453)\n  free_discovery_auth: sign-in-with-x wallet signature (chains, networks/status, arkm/circulating)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arkham/refs/heads/main/authentication/arkham-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Blockchain
- Blockchain Intelligence
- On-Chain Analytics
- Entity Attribution
- Wallet Intelligence
- Market Data
- DeFi
- Risk Scoring
---
