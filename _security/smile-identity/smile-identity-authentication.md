---
api_key_in:
- header
api_specs:
- filename: smile-identity-v3-openapi.json
  format: json
  label: Smile ID V3 API
  slug: smile-id-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/openapi/smile-identity-v3-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Smile Identity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smile Identity secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Smile Identity
provider_slug: smile-identity
scheme_count: 4
schemes:
- description: smileid-partner-id and smileid-api-key headers POSTed to /v3/token to mint a signed JWT access token (15-minute expiry). Keys are environment-specific (sandbox vs production) and must never be exposed client-side.
  headers:
  - smileid-partner-id
  - smileid-api-key
  in: header
  name: token-mint
  sources:
  - openapi/smile-identity-v3-openapi.json
  token_endpoint: https://api.smileidentity.com/v3/token
  type: apiKey
- description: JWT bearer token (from /v3/token) sent on all V3 verification requests.
  in: header
  name: SmileIDToken
  parameter_name: SmileID-Token
  sources:
  - openapi/smile-identity-v3-openapi.json
  type: apiKey
- description: Numeric partner identifier accompanying the token on each request.
  in: header
  name: SmileID-Partner-ID
  parameter_name: SmileID-Partner-ID
  sources:
  - openapi/smile-identity-v3-openapi.json
  type: apiKey
- description: Optional HMAC signature of the raw request body using the SDK/partner secret with SmileID-Timestamp as salt, sent in SmileID-Request-Signature. Required only when the account uses SDK/partner-secret HMAC authentication.
  headers:
  - SmileID-Timestamp
  - SmileID-Request-Signature
  name: hmac-signature
  scheme: hmac
  sources:
  - openapi/smile-identity-v3-openapi.json
  - https://docs.usesmileid.com/api-reference/authentication
  type: http
slug: smile-identity-authentication
source_filename: smile-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.usesmileid.com/api-reference/authentication\ndocs: https://docs.usesmileid.com/api-reference/authentication\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  model: >-\n    Two-legged: a server-side API key + partner ID mint a short-lived JWT via\n    POST /v3/token; that JWT is then sent as the SmileID-Token header on every\n    verification request. An optional HMAC request signature (SmileID-Timestamp\n    + SmileID-Request-Signature) is required when the account is configured for\n    SDK/partner-secret HMAC authentication.\nschemes:\n- name: token-mint\n  type: apiKey\n  in: header\n  description: >-\n    smileid-partner-id and smileid-api-key headers POSTed to /v3/token to mint a\n    signed JWT access token (15-minute expiry). Keys are environment-specific\n    (sandbox vs production) and must never be exposed client-side.\n  headers: [smileid-partner-id, smileid-api-key]\n\
  \  token_endpoint: https://api.smileidentity.com/v3/token\n  sources: [openapi/smile-identity-v3-openapi.json]\n- name: SmileIDToken\n  type: apiKey\n  in: header\n  parameter_name: SmileID-Token\n  description: JWT bearer token (from /v3/token) sent on all V3 verification requests.\n  sources: [openapi/smile-identity-v3-openapi.json]\n- name: SmileID-Partner-ID\n  type: apiKey\n  in: header\n  parameter_name: SmileID-Partner-ID\n  description: Numeric partner identifier accompanying the token on each request.\n  sources: [openapi/smile-identity-v3-openapi.json]\n- name: hmac-signature\n  type: http\n  scheme: hmac\n  description: >-\n    Optional HMAC signature of the raw request body using the SDK/partner secret\n    with SmileID-Timestamp as salt, sent in SmileID-Request-Signature. Required\n    only when the account uses SDK/partner-secret HMAC authentication.\n  headers: [SmileID-Timestamp, SmileID-Request-Signature]\n  sources: [openapi/smile-identity-v3-openapi.json, https://docs.usesmileid.com/api-reference/authentication]\n\
  token:\n  format: JWT\n  expiry_minutes: 15\n  environment_scoped: true\nnotes: >-\n  No OAuth2 / OpenID Connect surface — Smile ID uses API-key-minted JWT tokens\n  plus optional HMAC request signing, so there is no OAuth scopes artifact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smile-identity/refs/heads/main/authentication/smile-identity-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Identity Verification
- KYC
- KYB
- Biometrics
- Liveness Detection
- Document Verification
- AML
- Fraud Prevention
- Compliance
- Onboarding
- Africa
---
