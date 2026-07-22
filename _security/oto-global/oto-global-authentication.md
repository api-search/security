---
api_key_in: []
api_specs:
- filename: oto-global-openapi.yml
  format: yaml
  label: OTO API V2
  slug: oto-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oto-global/refs/heads/main/openapi/oto-global-openapi.yml
auth_types:
- http
description: 'OTO uses a two-token bearer scheme. A long-lived refresh_token is issued from the OTO dashboard (Settings -> API Integrations -> Connect). The refresh_token is exchanged at POST /rest/v2/refreshToken for a short-lived access_token (JWT, expires_in 3600s / 1 hour). All other endpoints are called with header Authorization: Bearer <access_token>. A small number of endpoints (refreshToken, healthCheck, register) require no auth.'
kind: authentication
layout: security
method: searched
name: Oto Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: OTO Global secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OTO Global
provider_slug: oto-global
scheme_count: 1
schemes:
- applies_to: all endpoints except refreshToken, healthCheck, register
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oto-global-openapi.yml
  type: http
slug: oto-global-authentication
source_filename: oto-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://apis.tryoto.com/ (OTO API V2 Authorization docs + Postman collection)\ndocs: https://help.tryoto.com/en/support/solutions/articles/150000178771\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  token_format: JWT\n  flow: refresh-token\n  api_key_in: []\n  oauth2_flows: []\ndescription: >-\n  OTO uses a two-token bearer scheme. A long-lived refresh_token is issued from the OTO\n  dashboard (Settings -> API Integrations -> Connect). The refresh_token is exchanged at\n  POST /rest/v2/refreshToken for a short-lived access_token (JWT, expires_in 3600s /\n  1 hour). All other endpoints are called with header Authorization: Bearer <access_token>.\n  A small number of endpoints (refreshToken, healthCheck, register) require no auth.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: all endpoints except refreshToken, healthCheck, register\n    sources: [openapi/oto-global-openapi.yml]\n\
  token_endpoint:\n  operation: refreshToken\n  method: POST\n  url: https://api.tryoto.com/rest/v2/refreshToken\n  request: '{ \"refresh_token\": \"<your refresh token>\" }'\n  response_fields: [access_token, refresh_token, token_type (Bearer), expires_in (3600), success]\n  obtain_refresh_token: OTO dashboard -> Settings -> API Integrations -> Connect\nnotes:\n  - access_token lifetime is 1 hour; renew via refreshToken before expiry.\n  - Tracking (public branded tracking URL) can be consumed without authorization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oto-global/refs/heads/main/authentication/oto-global-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Shipping
- Logistics
- Fulfillment
- E-commerce
- Delivery
- Carriers
- Returns
- Saudi Arabia
---
