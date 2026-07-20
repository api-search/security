---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dynamic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamic secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dynamic
provider_slug: dynamic
scheme_count: 2
schemes:
- description: Project/API bearer tokens generated in the Dynamic dashboard, used to authenticate admin and environment-management REST endpoints.
  format: Bearer <token>
  header: Authorization
  in: header
  name: Tokens
  scheme: bearer
  sources:
  - https://www.dynamic.xyz/docs/api-reference
  type: http
- description: User-scoped API tokens for calling user/SDK-facing endpoints on behalf of an authenticated end user.
  format: Bearer <token>
  header: Authorization
  in: header
  name: UserApiTokens
  scheme: bearer
  sources:
  - https://www.dynamic.xyz/docs/api-reference
  type: http
slug: dynamic-authentication
source_filename: dynamic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.dynamic.xyz/docs/api-reference\ndocs: https://www.dynamic.xyz/docs/api-reference\nnotes: >-\n  Derived from the Dynamic REST API reference (per-endpoint OpenAPI fragments).\n  No single machine-readable OpenAPI document is published; the reference is\n  split across ~944 doc pages. The API uses bearer API tokens issued from the\n  Dynamic dashboard. Two named token schemes appear: dashboard project/API\n  Tokens (admin endpoints) and User API Tokens (user-scoped access).\nsummary:\n  types: [http]\n  http_scheme: bearer\n  bearer_source: dashboard-issued API tokens\n  api_key_in: [header]\n  header: Authorization\n  oauth2_flows: []\nschemes:\n- name: Tokens\n  type: http\n  scheme: bearer\n  description: >-\n    Project/API bearer tokens generated in the Dynamic dashboard, used to\n    authenticate admin and environment-management REST endpoints.\n  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n\
  \  sources: [https://www.dynamic.xyz/docs/api-reference]\n- name: UserApiTokens\n  type: http\n  scheme: bearer\n  description: >-\n    User-scoped API tokens for calling user/SDK-facing endpoints on behalf of an\n    authenticated end user.\n  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n  sources: [https://www.dynamic.xyz/docs/api-reference]\nend_user_auth:\n  description: >-\n    End-user authentication (the product surface, distinct from API access) is\n    handled by the SDKs and supports email/SMS OTP, social/OAuth login,\n    passkeys, external wallet connection, and MFA (authenticator app, SMS,\n    passkeys, email OTP, TOTP). JWTs issued to end users are verifiable and an\n    External JWT admin endpoint exists for BYO-auth setups.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic/refs/heads/main/authentication/dynamic-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Wallet Infrastructure
- Web3
- Crypto
- Authentication
- Embedded Wallets
- Stablecoins
- Key Management
- MPC
- Developer Tools
- Fintech
- Blockchain
---
