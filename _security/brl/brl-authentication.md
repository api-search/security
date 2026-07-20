---
api_key_in:
- header
api_specs:
- filename: brl-openapi-original.json
  format: json
  label: Crown API & Webhooks
  slug: crown-api-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brl/refs/heads/main/openapi/brl-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Brl Authentication
name_suffix: Authentication
oauth_flows: []
overview: BRL secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BRL
provider_slug: brl
scheme_count: 3
schemes:
- algorithm: RS256
  bearerFormat: JWT
  description: 'Self-signed, per-request JWT. Signed with the partner''s private key using RS256 and sent as `Authorization: Bearer <jwt>`. Expiry must be within 50 seconds of issuance (exp - iat <= 50s). Required claims bind the token to a single request.'
  jwt_claims:
    bodyHash: SHA-256 hash of the request body
    exp: Unix timestamp of expiry (<= iat + 50s)
    iat: Unix timestamp of token creation
    nonce: Unique per-request identifier (replay protection)
    sub: The API key identifier
    uri: The endpoint path being accessed
  max_lifetime_seconds: 50
  name: JwtAuth
  scheme: bearer
  sources:
  - openapi/brl-openapi-original.json
  - https://docs.crown-brlv.com/guides/authentication
  type: http
- description: The account API key identifier, created via the API Keys Setup guide. Sent alongside the JWT on every request.
  docs: https://docs.crown-brlv.com/guides/api-keys-setup
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/brl-openapi-original.json
  - https://docs.crown-brlv.com/guides/authentication
  type: apiKey
- description: Webhook authentication only. HMAC-SHA256 signature of the request body computed with the account's webhook secret; verify it to confirm a webhook was sent by Crown.
  in: header
  name: signature
  parameter: X-Crown-Signature
  scope: webhooks
  sources:
  - openapi/brl-openapi-original.json
  type: apiKey
slug: brl-authentication
source_filename: brl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/brl-openapi-original.json\ndocs: https://docs.crown-brlv.com/guides/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: >-\n    Every authenticated request carries BOTH an X-API-Key header (the API key\n    identifier) AND a short-lived, self-signed RS256 JWT in the Authorization:\n    Bearer header. Crown does NOT issue tokens from a token endpoint — the\n    partner mints and signs the JWT locally with its private key. Webhook\n    deliveries are authenticated separately with an X-Crown-Signature HMAC.\nschemes:\n- name: JwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Self-signed, per-request JWT. Signed with the partner's private key using\n    RS256 and sent as `Authorization: Bearer <jwt>`. Expiry must be within 50\n    seconds of issuance (exp - iat <= 50s). Required claims bind the token to a\n    single request.\n  jwt_claims:\n \
  \   uri: The endpoint path being accessed\n    nonce: Unique per-request identifier (replay protection)\n    iat: Unix timestamp of token creation\n    exp: Unix timestamp of expiry (<= iat + 50s)\n    sub: The API key identifier\n    bodyHash: SHA-256 hash of the request body\n  algorithm: RS256\n  max_lifetime_seconds: 50\n  sources:\n  - openapi/brl-openapi-original.json\n  - https://docs.crown-brlv.com/guides/authentication\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: The account API key identifier, created via the API Keys Setup guide. Sent alongside the JWT on every request.\n  docs: https://docs.crown-brlv.com/guides/api-keys-setup\n  sources:\n  - openapi/brl-openapi-original.json\n  - https://docs.crown-brlv.com/guides/authentication\n- name: signature\n  type: apiKey\n  in: header\n  parameter: X-Crown-Signature\n  description: >-\n    Webhook authentication only. HMAC-SHA256 signature of the request body\n    computed with the account's\
  \ webhook secret; verify it to confirm a webhook\n    was sent by Crown.\n  scope: webhooks\n  sources:\n  - openapi/brl-openapi-original.json\ncapabilities_note: >-\n  Authorization within an account is capability-scoped rather than OAuth-scoped:\n  operations require account capabilities such as `manage-holders` (sub-account\n  management) and `auto-claim-rewards` (recurring reward claims). These are\n  account grants, not OAuth2 scopes, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brl/refs/heads/main/authentication/brl-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Crypto
- Stablecoin
- Payments
- Brazil
- PIX
- Fintech
- Blockchain
- Digital Assets
- Wallets
- Yield
---
