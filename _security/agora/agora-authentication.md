---
api_key_in: []
api_specs:
- filename: agora-openapi-original.yml
  format: yaml
  label: Agora Public API
  slug: agora-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/openapi/agora-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Agora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agora secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agora
provider_slug: agora
scheme_count: 2
schemes:
- description: 'Long-lived Agora access key (API key), sent as `Authorization: Bearer <accessKey>`. Used ONLY by POST /v0/auth/token to mint a short-lived session JWT. API keys are issued by Agora on request during Beta.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/agora-openapi-original.yml
  type: http
- bearerFormat: JWT
  description: 'Short-lived session JWT returned by POST /v0/auth/token, sent as `Authorization: Bearer <sessionJwt>` on every subsequent authenticated request. Valid for 15 minutes (fixed TTL, not echoed in the response). RS256-signed; issuer https://api.agora.finance. No refresh-token endpoint — re-exchange the API key before expiry.'
  name: sessionJwt
  scheme: bearer
  sources:
  - openapi/agora-openapi-original.yml
  type: http
slug: agora-authentication
source_filename: agora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/agora-openapi-original.yml\ndocs: https://docs.agora.finance/api/authentication\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  model: api-key-exchanged-for-session-jwt\n  public_endpoints: [GET /v0/metrics, GET /v0/metrics/total-supply, GET /v0/metrics/circulating-supply]\nschemes:\n  - name: accessKey\n    type: http\n    scheme: bearer\n    description: >-\n      Long-lived Agora access key (API key), sent as `Authorization: Bearer <accessKey>`.\n      Used ONLY by POST /v0/auth/token to mint a short-lived session JWT. API keys are\n      issued by Agora on request during Beta.\n    sources: [openapi/agora-openapi-original.yml]\n  - name: sessionJwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Short-lived session JWT returned by POST /v0/auth/token, sent as\n      `Authorization: Bearer <sessionJwt>` on every subsequent authenticated request.\n      Valid for 15 minutes\
  \ (fixed TTL, not echoed in the response). RS256-signed;\n      issuer https://api.agora.finance. No refresh-token endpoint — re-exchange the\n      API key before expiry.\n    sources: [openapi/agora-openapi-original.yml]\nflow: >-\n  1. POST /v0/auth/token with Authorization: Bearer <API_KEY> (no body) -> { sessionJwt }.\n  2. Attach the JWT as Authorization: Bearer <sessionJwt> for 15 minutes.\n  3. On 401 with context.reason=token_expired, re-exchange the API key.\nerror_401_reasons: [missing_header, invalid_token, token_expired, token_revoked, unknown_tenant, missing_claim]\nnotes: >-\n  Two http-bearer schemes with distinct roles. Public metrics endpoints require no\n  authentication; Accounts, Routes, and Transactions require a valid session JWT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/authentication/agora-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Fintech
- Stablecoin
- Digital Dollar
- Payments
- Cryptocurrency
- Blockchain
- API
- AUSD
---
