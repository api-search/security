---
api_key_in:
- header
api_specs:
- filename: pred-openapi.yml
  format: yaml
  label: PRED Trading Platform API
  slug: pred-trading-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pred/refs/heads/main/openapi/pred-openapi.yml
auth_types:
- http
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Pred Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pred secures its APIs with http, apiKey, and signature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pred
provider_slug: pred
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: 'JWT access token returned by POST /api/v1/auth/login-with-signature; sent as Authorization: Bearer <token>.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pred-openapi.yml
  type: http
- description: Partner API key required only for POST /api/v1/auth/login-with-signature. Requested directly from Pred (not self-service).
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - https://pred-1.gitbook.io/pred-docs/api-reference/authentication
  type: apiKey
- description: Login proof. EOA signs an EIP-712 CreateProxy message (domain "Pred Contract Proxy Factory", chainId + verifyingContract are env-specific). Signature format 0x<r><s><v>, low-s normalized.
  name: EIP712-CreateProxy
  scheme: eip-712
  sources:
  - https://pred-1.gitbook.io/pred-docs/api-reference/authentication
  type: signature
- description: Per-order authorization. EOA signs an EIP-712 Order message (domain "Pred CTF Exchange" version 1; verifyingContract = the parent market's contract_address from market discovery) for every order placement.
  name: EIP712-Order
  scheme: eip-712
  sources:
  - https://pred-1.gitbook.io/pred-docs/api-reference/orders
  type: signature
slug: pred-authentication
source_filename: pred-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pred-openapi.yml\ndocs: https://pred-1.gitbook.io/pred-docs/api-reference/authentication\nsummary:\n  types:\n  - http\n  - apiKey\n  - signature\n  api_key_in:\n  - header\n  notes: >-\n    Wallet-signature login. A partner-issued X-API-Key gates the\n    login-with-signature endpoint; the login itself is an EIP-712 CreateProxy\n    signature from the user's EOA. Successful login returns a short-lived JWT\n    access token (Bearer) plus a rotating refresh token; authenticated trading\n    endpoints additionally require X-Wallet-Address and X-Proxy-Address headers.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT access token returned by POST /api/v1/auth/login-with-signature; sent as Authorization: Bearer <token>.'\n  sources:\n  - openapi/pred-openapi.yml\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Partner API\
  \ key required only for POST /api/v1/auth/login-with-signature.\n    Requested directly from Pred (not self-service).\n  sources:\n  - https://pred-1.gitbook.io/pred-docs/api-reference/authentication\n- name: EIP712-CreateProxy\n  type: signature\n  scheme: eip-712\n  description: >-\n    Login proof. EOA signs an EIP-712 CreateProxy message (domain\n    \"Pred Contract Proxy Factory\", chainId + verifyingContract are env-specific).\n    Signature format 0x<r><s><v>, low-s normalized.\n  sources:\n  - https://pred-1.gitbook.io/pred-docs/api-reference/authentication\n- name: EIP712-Order\n  type: signature\n  scheme: eip-712\n  description: >-\n    Per-order authorization. EOA signs an EIP-712 Order message (domain\n    \"Pred CTF Exchange\" version 1; verifyingContract = the parent market's\n    contract_address from market discovery) for every order placement.\n  sources:\n  - https://pred-1.gitbook.io/pred-docs/api-reference/orders\ncontext_headers:\n- name: X-Wallet-Address\n  usage:\
  \ EOA wallet address; required on order and portfolio endpoints.\n- name: X-Proxy-Address\n  usage: Gnosis Safe proxy wallet address; required on order and portfolio endpoints.\n- name: X-Refresh-Token\n  usage: Refresh token for POST /api/v1/auth/refresh/token (or refresh_token cookie).\ntoken_lifecycle:\n  refresh_endpoint: POST /api/v1/auth/refresh/token\n  rotation: Each refresh rotates the refresh token; reusing an old one returns 401 REFRESH_TOKEN_ALREADY_USED.\n  sdk_refresh_threshold_seconds: 300\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pred/refs/heads/main/authentication/pred-authentication.yml
summary_line: http/apiKey/signature · 4 schemes
tags:
- Company
- Fintech
- Prediction Markets
- Sports
- Trading
- Exchange
- Web3
- Blockchain
- Base
- USDC
---
