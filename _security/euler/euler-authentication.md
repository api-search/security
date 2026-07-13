---
api_key_in:
- cookie
- header
api_specs:
- filename: openapi.json
  format: json
  label: Euler V3 Data API
  slug: euler-v3-data-api
  spec_type: OpenAPI
  url: https://v3.euler.finance/v3/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Euler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Euler Finance secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Euler Finance
provider_slug: euler
scheme_count: 5
schemes:
- description: API key authentication (optional; higher rate limits).
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
- bearerFormat: API key
  description: 'Alternative to X-API-Key using Authorization: Bearer <key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/euler-v3-data-api.json
  type: http
- description: Admin secret (server-to-server) for API key management.
  in: header
  name: AdminSecret
  parameter: X-Admin-Secret
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
- description: Signed, httpOnly platform-operator browser session cookie.
  in: cookie
  name: PlatformSession
  parameter: euler_platform_session
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
- description: Double-submit CSRF token required for unsafe cookie-authenticated methods.
  in: header
  name: PlatformCsrf
  parameter: X-CSRF-Token
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
slug: euler-authentication
source_filename: euler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/euler-v3-data-api.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key authentication (optional; higher rate limits).\n  sources:\n  - openapi/euler-v3-data-api.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Alternative to X-API-Key using Authorization: Bearer <key>'\n  sources:\n  - openapi/euler-v3-data-api.json\n- name: AdminSecret\n  type: apiKey\n  in: header\n  parameter: X-Admin-Secret\n  description: Admin secret (server-to-server) for API key management.\n  sources:\n  - openapi/euler-v3-data-api.json\n- name: PlatformSession\n  type: apiKey\n  in: cookie\n  parameter: euler_platform_session\n  description: Signed, httpOnly platform-operator browser session cookie.\n  sources:\n  - openapi/euler-v3-data-api.json\n- name:\
  \ PlatformCsrf\n  type: apiKey\n  in: header\n  parameter: X-CSRF-Token\n  description: Double-submit CSRF token required for unsafe cookie-authenticated methods.\n  sources:\n  - openapi/euler-v3-data-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/authentication/euler-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- DeFi
- Lending
- Borrowing
- Finance
- Ethereum
- Blockchain
- Vaults
- Liquidation
- Interest Rates
- Permissionless
---
