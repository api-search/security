---
api_key_in:
- header
api_specs:
- filename: metalend-rebalancing-openapi.json
  format: json
  label: MetaLend Rebalancing API
  slug: metalend-rebalancing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-rebalancing-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Metalend Authentication
name_suffix: Authentication
oauth_flows: []
overview: MetaLend secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MetaLend
provider_slug: metalend
scheme_count: 3
schemes:
- description: API key required for all endpoints.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/metalend-rebalancing-openapi.json
  type: apiKey
- description: 'JWT issued by POST /v1/auth/verify. Pass as Authorization: Bearer <token>.


    x-agent-hint: agentcash and other agentic wallets strip the Authorization header for their own SIWX flow. Use X-MetaLend-JWT: Bearer <token> instead — the backend accepts both headers. Affected endpoints: POST /v1/deposits, POST /v1/withdrawals, PUT /v1/config.'
  in: header
  name: JwtAuth
  parameter: Authorization
  sources:
  - openapi/metalend-rebalancing-openapi.json
  type: apiKey
- description: 'Required for CORS requests from browsers. Must match the allowed origins configured for the API key. Example: Origin: https://app.metalend.tech. Localhost is always allowed but must be specified.'
  in: header
  name: OriginHeader
  parameter: Origin
  sources:
  - openapi/metalend-rebalancing-openapi.json
  type: apiKey
slug: metalend-authentication
source_filename: metalend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/metalend-rebalancing-openapi.json\ndocs: https://api.metalend.tech/SKILL.md\nportal: https://developer.metalend.tech\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    Every endpoint requires X-API-Key + Origin. Deposits, withdrawals, and config\n    updates additionally require a JWT obtained via a SIWE (EIP-4361) challenge/verify\n    flow; the JWT is sent as Authorization: Bearer <jwt> or, for agentic wallets that\n    strip Authorization, as X-MetaLend-JWT: Bearer <jwt>. Value-moving calls also carry\n    wallet signatures (EIP-191/EIP-712/EIP-3009). Get an API key at the developer portal.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key required for all endpoints.\n  sources:\n  - openapi/metalend-rebalancing-openapi.json\n- name: JwtAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    JWT issued\
  \ by POST /v1/auth/verify. Pass as Authorization: Bearer <token>.\n\n    x-agent-hint: agentcash and other agentic wallets strip the Authorization header for their own SIWX flow. Use X-MetaLend-JWT: Bearer <token> instead — the backend accepts both headers. Affected endpoints: POST /v1/deposits, POST /v1/withdrawals, PUT /v1/config.\n  sources:\n  - openapi/metalend-rebalancing-openapi.json\n- name: OriginHeader\n  type: apiKey\n  in: header\n  parameter: Origin\n  description: 'Required for CORS requests from browsers. Must match the allowed origins configured\n    for the API key. Example: Origin: https://app.metalend.tech. Localhost is always allowed\n    but must be specified.'\n  sources:\n  - openapi/metalend-rebalancing-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/authentication/metalend-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Crypto
- DeFi
- Lending
- Yield
- Rebalancing
- Web3
- Stablecoins
- Payments
- Agent Native
- Blockchain
---
