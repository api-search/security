---
api_key_in:
- header
api_specs:
- filename: tzero-issuance-secondary-markets-openapi.json
  format: json
  label: tZERO Issuance & Secondary Markets API
  slug: issuance-secondary-markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tzero/refs/heads/main/openapi/tzero-issuance-secondary-markets-openapi.json
- filename: tzero-institutional-openapi.json
  format: json
  label: tZERO Institutional API
  slug: institutional
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tzero/refs/heads/main/openapi/tzero-institutional-openapi.json
auth_types:
- apiKey
- http
- refreshToken
description: ''
kind: authentication
layout: security
method: searched
name: Tzero Authentication
name_suffix: Authentication
oauth_flows: []
overview: tZERO secures its APIs with apiKey, http, and refreshToken across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: tZERO
provider_slug: tzero
scheme_count: 4
schemes:
- description: API key generated at app.t0kenizer.com/ta/api-keys
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/tzero-institutional-openapi.json
  type: apiKey
- in: header
  name: x-api-key
  parameter: x-apikey
  sources:
  - openapi/tzero-issuance-secondary-markets-openapi.json
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tzero-issuance-secondary-markets-openapi.json
  type: http
- name: refreshToken
  sources:
  - openapi/tzero-issuance-secondary-markets-openapi.json
  type: refreshToken
slug: tzero-authentication
source_filename: tzero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: openapi/tzero-institutional-openapi.json, openapi/tzero-issuance-secondary-markets-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - refreshToken\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key generated at app.t0kenizer.com/ta/api-keys\n  sources:\n  - openapi/tzero-institutional-openapi.json\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  sources:\n  - openapi/tzero-issuance-secondary-markets-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tzero-issuance-secondary-markets-openapi.json\n- name: refreshToken\n  type: refreshToken\n  sources:\n  - openapi/tzero-issuance-secondary-markets-openapi.json\ndocs: https://apidocs.tzero.com/docs\nnote: 'Derived from both OpenAPI contracts, then upgraded from the tZERO API docs. The two surfaces do NOT\
  \ share\n  credentials. Note the \"refreshToken\" scheme in the Issuance & Secondary Markets contract declares type: refreshToken,\n  which is not a valid OpenAPI securityScheme type — it is a vendor value, recorded verbatim.'\nsurfaces:\n- surface: issuance-secondary-markets\n  base_url: https://gateway-web-api.tzero.com/app\n  style: api-key + bearer JWT\n  headers:\n  - x-apikey\n  - 'Authorization: Bearer <accessToken>'\n  token_endpoint: POST /auth/v1/api/token\n  refresh_endpoint: POST /auth/v1/api/refresh\n  token_lifetime: 1 hour\n  key_issuance: contact tZERO — no self-serve API signup\n  docs: https://apidocs.tzero.com/docs\n- surface: institutional\n  base_url: https://api.t0direct.com/api/v1\n  style: api-key\n  headers:\n  - X-API-Key\n  key_prefix: t0k_\n  scoped: true\n  key_issuance: app.t0kenizer.com/ta/api-keys (host did not resolve in DNS on 2026-09-01)\n  insufficient_scope_status: 403\n  docs: https://api.t0direct.com/api/v1/docs/\npermissions:\n  note: The Institutional\
  \ API publishes a named permission model in its OpenAPI info.description. These are API-key\n    scopes, not OAuth scopes — tZERO declares no oauth2 securityScheme anywhere, so no scopes/ artifact is emitted.\n  source: openapi/tzero-institutional-openapi.json#/info/description\n  scopes:\n  - scope: TA_READ\n    group: Transfer Agent\n    description: Read investors, securities, holdings, documents, dividends, corporate actions, proposals\n  - scope: TA_WRITE\n    group: Transfer Agent\n    description: Create/update investors, submit issuances, declare dividends and corporate actions, create voting\n      proposals\n  - scope: TA_TRANSFERS\n    group: Transfer Agent\n    description: Submit and manage book-entry transfers\n  - scope: TA_ADMIN\n    group: Transfer Agent\n    description: Administrative transfer-agent operations\n  - scope: TOKENS_READ\n    group: Tokenization\n    description: Read token configurations and deployments\n  - scope: DEPLOYMENTS_READ\n    group: Tokenization\n\
  \    description: Read deployments and operation history\n  - scope: CUSTODY_READ\n    group: Custody\n    description: Read vaults, balances, transfers and whitelisted addresses\n  - scope: FULL_ACCESS\n    group: Master\n    description: Satisfies all scopes — the contract says to use it sparingly\n  reserved_scopes:\n  - TOKENS_WRITE\n  - DEPLOYMENTS_WRITE\n  - PRICE_WRITE\n  - CUSTODY_WRITE\n  - CAPTABLE_*\n  reserved_note: present in the enum but not exposed to customers today\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tzero/refs/heads/main/authentication/tzero-authentication.yml
summary_line: apiKey/http/refreshToken · 4 schemes
tags:
- Company
- Digital Securities
- Tokenization
- Capital Markets
- Trading
- Alternative Trading System
- Transfer Agent
- Custody
- Blockchain
- Financial Services
- Securities
- Market Data
- FIX Protocol
---
