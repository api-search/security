---
api_key_in: []
api_specs:
- filename: classic-shapeshift-openapi-original.json
  format: json
  label: ShapeShift Public API
  slug: shapeshift-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/openapi/classic-shapeshift-openapi-original.json
auth_types:
- siwe
- http-bearer-jwt
description: ''
kind: authentication
layout: security
method: searched
name: Classic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Classic secures its APIs with siwe and http-bearer-jwt across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Classic
provider_slug: classic
scheme_count: 3
schemes:
- flow:
  - POST /v1/auth/siwe/nonce (siweNonce) -> nonce
  - Wallet signs the SIWE message containing the nonce
  - POST /v1/auth/siwe/verify (siweVerify) -> { token (JWT), address }
  name: SIWE
  sources:
  - openapi/classic-shapeshift-openapi-original.json
  standard: EIP-4361 (Sign-In With Ethereum)
  type: siwe
- applies_to:
  - createAffiliate
  - updateAffiliate
  bearerFormat: JWT
  description: JWT returned by siweVerify, sent as Authorization Bearer on authenticated affiliate operations (401/403 on failure).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/classic-shapeshift-openapi-original.json
  type: http
- applies_to:
  - getSwapQuote
  - getSwapRates
  - getSwapStatus
  description: Partner/affiliate code passed on swap endpoints for attribution; not an authentication credential.
  in: header
  name: X-Partner-Code
  parameter: X-Partner-Code
  role: attribution
  sources:
  - openapi/classic-shapeshift-openapi-original.json
  type: apiKey
slug: classic-authentication
source_filename: classic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.shapeshift.com/docs\nnotes: >-\n  The ShapeShift Public API does not declare securitySchemes in its OpenAPI, but\n  authentication is documented through its Auth operations: Sign-In With Ethereum\n  (SIWE, EIP-4361). A client fetches a nonce (siweNonce), the wallet signs the\n  SIWE message, and siweVerify returns a JWT bearer token used on authenticated\n  endpoints (affiliate create/update). Read endpoints (assets, chains, swap\n  quotes/rates/status) are public. Swap and affiliate endpoints also accept an\n  X-Partner-Code header for partner/affiliate attribution (not authentication).\nsummary:\n  types: [siwe, http-bearer-jwt]\n  public_endpoints: true\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: SIWE\n    type: siwe\n    standard: EIP-4361 (Sign-In With Ethereum)\n    flow:\n      - \"POST /v1/auth/siwe/nonce (siweNonce) -> nonce\"\n      - \"Wallet signs the SIWE message containing the nonce\"\
  \n      - \"POST /v1/auth/siwe/verify (siweVerify) -> { token (JWT), address }\"\n    sources: [openapi/classic-shapeshift-openapi-original.json]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: JWT returned by siweVerify, sent as Authorization Bearer on authenticated affiliate operations (401/403 on failure).\n    applies_to: [createAffiliate, updateAffiliate]\n    sources: [openapi/classic-shapeshift-openapi-original.json]\n  - name: X-Partner-Code\n    type: apiKey\n    in: header\n    parameter: X-Partner-Code\n    role: attribution\n    description: Partner/affiliate code passed on swap endpoints for attribution; not an authentication credential.\n    applies_to: [getSwapQuote, getSwapRates, getSwapStatus]\n    sources: [openapi/classic-shapeshift-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classic/refs/heads/main/authentication/classic-authentication.yml
summary_line: siwe/http-bearer-jwt · 3 schemes
tags:
- Company
- Crypto
- Cryptocurrency
- DEX Aggregator
- Swaps
- Blockchain
- Wallet
- Self-Custody
---
