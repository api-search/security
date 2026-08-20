---
api_key_in:
- header
api_specs:
- filename: magnite-springserve-v1-openapi.yml
  format: yaml
  label: SpringServe UI API
  slug: springserve-ui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magnite/refs/heads/main/openapi/magnite-springserve-v1-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Magnite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magnite secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Magnite
provider_slug: magnite
scheme_count: 2
schemes:
- description: SpringServe authorization token based authentication.
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/magnite-springserve-v0-openapi.yml
  - openapi/magnite-springserve-v1-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: SpringServe authorization bearer token based authentication.  This key is included in the response from the /api/v0/auth and /api/v1/auth endpoints.  This key will be automatically set if you run the example for /api/v0/auth or /api/v1/auth
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/magnite-springserve-v0-openapi.yml
  - openapi/magnite-springserve-v1-openapi.yml
  type: http
slug: magnite-authentication
source_filename: magnite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.springserve.com/api-docs/swagger/v1/swagger.yaml (info.description Authentication\n  section), openapi/magnite-springserve-v0-openapi.yml, openapi/magnite-springserve-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: SpringServe authorization token based authentication.\n  sources:\n  - openapi/magnite-springserve-v0-openapi.yml\n  - openapi/magnite-springserve-v1-openapi.yml\n- name: bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: SpringServe authorization bearer token based authentication.  This key is included in the\n    response from the /api/v0/auth and /api/v1/auth endpoints.  This key will be automatically set if\n    you run the example for /api/v0/auth or /api/v1/auth\n  sources:\n  - openapi/magnite-springserve-v0-openapi.yml\n  - openapi/magnite-springserve-v1-openapi.yml\n\
  docs: https://api.springserve.com/api-docs\nnote: 'SpringServe mints its own tokens rather than using OAuth. POST /api/v0/auth or POST /api/v1/auth\n  takes an application/x-www-form-urlencoded body of email + password and returns a token usable two ways:\n  as a raw token in \"Authorization: <token>\" (scheme api_key) or as a JWT in \"Authorization: Bearer <token>\"\n  (scheme bearer_token). There is no oauth2 or openIdConnect scheme in either document, so there is no\n  scope surface and no scopes/ artifact — permissions are account- and role-based instead, readable at\n  GET /api/v1/accounts/permissions and per-collection ..._permissions_get operations. The hosted Swagger\n  UI at api.springserve.com/api-docs additionally falls back to the browser SpringServe session cookie,\n  but that is a docs-console convenience, not an API auth mode. Every request also runs against a server-side\n  ACTIVE ACCOUNT (GET /api/v1/accounts/current, POST /api/v1/accounts/{id}/set_current), which is effectively\n\
  \  a second half of the credential: the same token returns different data depending on the active account.'\ntoken_endpoints:\n- POST /api/v0/auth\n- POST /api/v1/auth\ncredential_grant: email + password exchanged for a token (application/x-www-form-urlencoded)\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  supported: false\n  model: account + role based permissions\n  read_at:\n  - GET /api/v1/accounts/permissions\n  - GET /api/v1/<collection>/permissions\nauthorization_context:\n  active_account_required: true\n  read: GET /api/v1/accounts/current\n  set: POST /api/v1/accounts/{id}/set_current\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magnite/refs/heads/main/authentication/magnite-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Advertising
- Programmatic Advertising
- Sell-Side Platform
- SSP
- Connected TV
- CTV
- OTT
- Streaming
- Display Advertising
- Video Advertising
- OpenRTB
- Header Bidding
- AdTech
- Publisher Monetization
- Demand-Side Integration
- Ad Server
- Deal Curation
- Reporting API
- Agent Readiness
- OpenAPI
---
