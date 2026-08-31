---
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: TronZap REST API
  slug: tronzap-rest-api
  spec_type: Postman
  url: https://www.postman.com/tron-energy/tronzap-com/overview
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tronzap Authentication
name_suffix: Authentication
oauth_flows: []
overview: TronZap declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: TronZap
provider_slug: tronzap
scheme_count: 3
schemes:
- api: TronZap REST API
  description: API token issued from the TronZap Dashboard (dash.tronzap.com) under the API section. Required on every /v1/* account endpoint.
  format: 'Authorization: Bearer <API_TOKEN>'
  in: header
  name: bearer_token
  parameter: Authorization
  scheme: bearer
  source: https://docs.tronzap.com/api/authentication.html
  type: http
- algorithm: SHA-256
  api: TronZap REST API
  description: Body-integrity signature accompanying the bearer token. Computed as sha256(raw_request_body + api_secret), hex-encoded. The provider publishes the identical construction in Bash, Node.js, PHP and Python. The secret is never transmitted, so this is a shared-secret HMAC-style construction rather than an ordinary API key.
  encoding: lowercase hex
  formula: sha256(<raw JSON request body> + <API_SECRET>)
  in: header
  name: request_signature
  parameter: X-Signature
  source: https://docs.tronzap.com/api/authentication.html
  type: apiKey
- api: TronZap Wallet Orders API
  description: The Orders API for non-custodial wallet integrations is explicitly public. The provider states "No authentication headers are required. The Orders API is fully public." Only Content-Type and Accept are required. Attribution is carried by an optional referral_code field in the request body, which credits partner commission but grants no access.
  name: none
  source: https://docs-wallets.tronzap.com/api/
  type: none
slug: tronzap-authentication
source_filename: tronzap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: >-\n  https://docs.tronzap.com/api/authentication.html and\n  https://docs-wallets.tronzap.com/api/ (Required headers), fetched 2026-08-30\ndocs: https://docs.tronzap.com/api/authentication.html\nnote: >-\n  TronZap has no OpenAPI, so this profile is read from the published authentication\n  reference rather than derived from securitySchemes. Two surfaces with opposite postures:\n  the account API is bearer + HMAC-signed, the wallet Orders API is completely\n  unauthenticated.\nschemes:\n- name: bearer_token\n  api: TronZap REST API\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <API_TOKEN>'\n  description: >-\n    API token issued from the TronZap Dashboard (dash.tronzap.com) under the API section.\n    Required on every /v1/* account endpoint.\n  source: https://docs.tronzap.com/api/authentication.html\n- name: request_signature\n  api: TronZap REST API\n  type:\
  \ apiKey\n  in: header\n  parameter: X-Signature\n  algorithm: SHA-256\n  description: >-\n    Body-integrity signature accompanying the bearer token. Computed as\n    sha256(raw_request_body + api_secret), hex-encoded. The provider publishes the identical\n    construction in Bash, Node.js, PHP and Python. The secret is never transmitted, so this\n    is a shared-secret HMAC-style construction rather than an ordinary API key.\n  formula: sha256(<raw JSON request body> + <API_SECRET>)\n  encoding: lowercase hex\n  source: https://docs.tronzap.com/api/authentication.html\n- name: none\n  api: TronZap Wallet Orders API\n  type: none\n  description: >-\n    The Orders API for non-custodial wallet integrations is explicitly public. The provider\n    states \"No authentication headers are required. The Orders API is fully public.\" Only\n    Content-Type and Accept are required. Attribution is carried by an optional\n    referral_code field in the request body, which credits partner commission\
  \ but grants\n    no access.\n  source: https://docs-wallets.tronzap.com/api/\nrequired_headers:\n  account_api:\n  - 'Authorization: Bearer YOUR_API_TOKEN'\n  - 'X-Signature: YOUR_SIGNATURE'\n  - 'Content-Type: application/json'\n  orders_api:\n  - 'Content-Type: application/json'\n  - 'Accept: application/json'\ncredential_issuance:\n  console: https://dash.tronzap.com/\n  path: Dashboard -> API section -> copy API token and secret\n  self_service: true\n  registration_required_for_orders_api: false\nobservations:\n- >-\n  The signature covers the exact serialized request body, so any client that re-serializes\n  JSON between signing and sending will fail with error code 1 (auth). The provider does not\n  publish a canonicalization rule, which makes this the most likely integration failure.\n- >-\n  There is no OAuth2, no OpenID Connect, no mutual TLS and no scope model on either surface.\n  Authorization is all-or-nothing per token.\n- >-\n  Authentication errors are returned as HTTP\
  \ 200 with body code 1 / key \"auth\", not as a 401.\nsummary:\n  auth_types: [http-bearer, shared-secret-signature, none]\n  api_key_locations: [header]\n  oauth2_flows: []\n  scopes_documented: false\n  surfaces_authenticated: 1\n  surfaces_public: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronzap/refs/heads/main/authentication/tronzap-authentication.yml
summary_line: 3 schemes
tags:
- Blockchain
- Cryptocurrency
- TRON
- DeFi infrastructure
- Stablecoin
- USDT
- TRC-20
- Resource marketplace
- Payments
- Fees optimization
- Web3
- DeFi
- Payouts
- Compliance
- AML
- Developer Tools
- SDK
---
