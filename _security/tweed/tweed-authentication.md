---
api_key_in: []
api_specs:
- filename: tweed-api-v2-openapi-original.json
  format: json
  label: Tweed API (V2)
  slug: tweed-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-api-v2-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tweed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tweed secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tweed
provider_slug: tweed
scheme_count: 2
schemes:
- bearerFormat: Bearer
  description: 'API (V2): create a User Access Token (API Key + API Secret) on the Management Dashboard (dashboard.paytweed.com/api-keys) and send it as "Authorization: Bearer <API_KEY>:<API_SECRET>" on every request.'
  name: bearer
  scheme: Bearer
  sources:
  - openapi/tweed-api-v2-openapi-original.json
  type: http
- bearerFormat: JWT
  description: 'API (V1): POST apiKey + apiSecret to https://api-console.paytweed.com/auth/getAccessToken to obtain a JWT, then send "Authorization: Bearer <JWT>" on calls to api-console.paytweed.com. Docs advise regenerating the JWT only on expiry, not per call.'
  docs: https://docs.paytweed.com/developer-tools/api/api-v1
  name: v1-jwt-bearer
  scheme: Bearer
  sources:
  - https://docs.paytweed.com/developer-tools/api/api-v1
  type: http
slug: tweed-authentication
source_filename: tweed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tweed-api-v2-openapi-original.json\ndocs: https://docs.paytweed.com/developer-tools/api/api-v2/authorization\nsummary:\n  types:\n  - http\n  patterns:\n  - bearer user-access-token (API key:secret)\n  - bearer JWT (v1)\nschemes:\n- name: bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: Bearer\n  description: >-\n    API (V2): create a User Access Token (API Key + API Secret) on the\n    Management Dashboard (dashboard.paytweed.com/api-keys) and send it as\n    \"Authorization: Bearer <API_KEY>:<API_SECRET>\" on every request.\n  sources:\n  - openapi/tweed-api-v2-openapi-original.json\n- name: v1-jwt-bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: >-\n    API (V1): POST apiKey + apiSecret to\n    https://api-console.paytweed.com/auth/getAccessToken to obtain a JWT, then\n    send \"Authorization: Bearer <JWT>\" on calls to api-console.paytweed.com.\n    Docs advise regenerating the\
  \ JWT only on expiry, not per call.\n  docs: https://docs.paytweed.com/developer-tools/api/api-v1\n  sources:\n  - https://docs.paytweed.com/developer-tools/api/api-v1\nnotes: >-\n  No OAuth2/OIDC surface (no oauth2 securityScheme; openid-configuration\n  absent). API keys are managed in the dashboard; the V2 API also exposes\n  key management operations (AuthController_generateApiToken,\n  AuthController_getApiKeys, AuthController_deleteApiKey). End-user wallet\n  auth in the SDKs is a separate social-login flow (Google) handled by the\n  core SDKs, not an API credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/authentication/tweed-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Payments
- Crypto
- Wallets
- NFT
- Blockchain
- Web3
- Checkout
---
