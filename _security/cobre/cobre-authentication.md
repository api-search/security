---
api_key_in:
- body
api_specs:
- filename: cobre-events-asyncapi.yml
  format: yaml
  label: Cobre Platform API
  slug: cobre-platform-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobre/refs/heads/main/asyncapi/cobre-events-asyncapi.yml
auth_types:
- http-bearer
- token-exchange
description: ''
kind: authentication
layout: security
method: searched
name: Cobre Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cobre secures its APIs with http-bearer and token-exchange across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cobre
provider_slug: cobre
scheme_count: 2
schemes:
- description: POST credentials (user_id + secret; QA uses client_id + client_secret) to the auth endpoint to obtain an access_token.
  name: token-exchange
  request_fields:
  - user_id
  - secret
  response_fields:
  - access_token
  - type
  - expiration_time
  sources:
  - docs
  token_endpoint: /v1/auth
  token_format: JWT
  token_ttl_seconds: 1200
  token_type: Bearer
  type: token-exchange
- bearerFormat: JWT
  description: 'Send the access_token from /v1/auth as `Authorization: Bearer <token>` on all subsequent requests. Tokens expire after 1200 seconds (20 min); the docs recommend caching and refreshing just-in-time with a 60-120s safety window and a mutex lock to avoid concurrent refreshes.'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
slug: cobre-authentication
source_filename: cobre-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cobre.com/authentication-1886552m0\ndocs: https://docs.cobre.com/authentication-1886552m0\nsummary:\n  types: [http-bearer, token-exchange]\n  api_key_in: [body]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    Cobre uses a credential-for-token exchange. The client posts long-lived\n    credentials to the auth endpoint and receives a short-lived JWT access\n    token that is then sent as a Bearer token on every API call. Cobre's\n    security page describes this as an OAuth 2.0 / JWT model; the developer\n    auth guide documents it as a credentials (user_id + secret) exchange.\nschemes:\n  - name: token-exchange\n    type: token-exchange\n    description: >-\n      POST credentials (user_id + secret; QA uses client_id + client_secret)\n      to the auth endpoint to obtain an access_token.\n    token_endpoint: /v1/auth\n    request_fields: [user_id, secret]\n    response_fields: [access_token, type, expiration_time]\n\
  \    token_type: Bearer\n    token_format: JWT\n    token_ttl_seconds: 1200\n    sources: [docs]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    header: Authorization\n    description: >-\n      Send the access_token from /v1/auth as `Authorization: Bearer <token>`\n      on all subsequent requests. Tokens expire after 1200 seconds (20 min);\n      the docs recommend caching and refreshing just-in-time with a 60-120s\n      safety window and a mutex lock to avoid concurrent refreshes.\n    sources: [docs]\nguidance:\n  - Store credentials in a secure vault; never expose in plain text.\n  - Rotate API secrets periodically (docs recommend monthly).\n  - Configure API IP whitelisting where available.\n  - QA credentials (client_id/client_secret) are requested from your Account Manager.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobre/refs/heads/main/authentication/cobre-authentication.yml
summary_line: http-bearer/token-exchange · 2 schemes
tags:
- Company
- Fintech
- Payments
- Treasury
- Money Movement
- Cross Border Payments
- FX
- Stablecoins
- Banking
- Latin America
- Colombia
- Mexico
---
