---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Eldorado Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eldorado secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eldorado
provider_slug: eldorado
scheme_count: 3
schemes:
- description: Unique identifier assigned to each API partner / client organization. Required on all requests. Issued by El Dorado after emailing api@eldorado.io. Has active/inactive status.
  in: header
  name: X-Client-ID
  parameter: X-Client-ID
  sources:
  - https://api.eldorado.io/authentication/client-credentials
  type: apiKey
- description: Identifies the integration source/channel bound to a ClientID. Source type is API or WIDGET. A ClientID may have multiple ReferralIDs. Required on all requests.
  in: header
  name: X-Referral-ID
  parameter: X-Referral-ID
  sources:
  - https://api.eldorado.io/authentication/client-credentials
  type: apiKey
- bearerFormat: JWT
  description: 'Per-user access token returned by /auth/login/verify-otp. Carried as ''Authorization: Bearer <token>''. Required for user-facing operations (KYC, order creation); optional on public quote endpoints. JWT payload includes sub (user id), cid (client id), rid (referral id). Token expires automatically; re-authenticate on expiry.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://api.eldorado.io/authentication/client-credentials
  type: http
slug: eldorado-authentication
source_filename: eldorado-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.eldorado.io/authentication/client-credentials\ndocs: https://api.eldorado.io/authentication/client-credentials\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  notes: >-\n    El Dorado uses partner-level credentials (ClientID + ReferralID) sent as request headers,\n    plus a per-user JWT bearer access token obtained through an email OTP login flow. There is\n    no OAuth2 authorization server; the JWT is minted by the login endpoints.\nschemes:\n- name: X-Client-ID\n  type: apiKey\n  in: header\n  parameter: X-Client-ID\n  description: >-\n    Unique identifier assigned to each API partner / client organization. Required on all\n    requests. Issued by El Dorado after emailing api@eldorado.io. Has active/inactive status.\n  sources: [https://api.eldorado.io/authentication/client-credentials]\n- name: X-Referral-ID\n  type: apiKey\n  in: header\n  parameter:\
  \ X-Referral-ID\n  description: >-\n    Identifies the integration source/channel bound to a ClientID. Source type is API or WIDGET.\n    A ClientID may have multiple ReferralIDs. Required on all requests.\n  sources: [https://api.eldorado.io/authentication/client-credentials]\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Per-user access token returned by /auth/login/verify-otp. Carried as\n    'Authorization: Bearer <token>'. Required for user-facing operations (KYC, order creation);\n    optional on public quote endpoints. JWT payload includes sub (user id), cid (client id),\n    rid (referral id). Token expires automatically; re-authenticate on expiry.\n  sources: [https://api.eldorado.io/authentication/client-credentials]\nflows:\n  login:\n    description: Email OTP login that mints the JWT bearer token.\n    steps:\n    - operation: POST /auth/login/send-otp\n      description: Send a one-time password to the user's email (requires\
  \ ClientID + ReferralID headers).\n    - operation: POST /auth/login/verify-otp\n      description: Verify the OTP and receive the JWT access token.\n  admin:\n    description: >-\n      Separate admin/backend flow for administrative and webhook operations (distinct from\n      user-facing endpoints), documented as using ClientID + API Keys.\ncredential_request:\n  contact: api@eldorado.io\n  required_information:\n  - Organization/Company name\n  - Integration type (API, Widget, or both)\n  - Technical contact information\n  - Use case description\n  - Expected integration timeline\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eldorado/refs/heads/main/authentication/eldorado-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Crypto Web3
- Stablecoins
- Payments
- Onramp
- Offramp
- Cryptocurrency
- Latin America
- KYC
- Compliance
- Fintech
- Trading
---
