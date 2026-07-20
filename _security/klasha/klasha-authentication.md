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
name: Klasha Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klasha secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Klasha
provider_slug: klasha
scheme_count: 2
schemes:
- description: Merchant public key, generated from the Klasha dashboard under Settings -> Generate API Keys -> Merchant public key. Sent as the value of the `x-auth-token` request header on every endpoint that requires it.
  in: header
  name: MerchantPublicKey
  obtain: https://dashboard.klasha.com/settings/keys
  parameter_name: x-auth-token
  source: https://developers.klasha.com/overview/authentication
  type: apiKey
- bearer_format: JWT
  description: Bearer token used as the value of the `Authorization` header. Issued by the account login endpoint in exchange for the account email (`username`) and `password`.
  name: BearerToken
  scheme: bearer
  source: https://developers.klasha.com/overview/authentication
  token_endpoint:
    base: '{{env_url}}'
    method: POST
    path: /auth/account/v2/login
    request_fields:
    - description: Your account email
      name: username
      required: true
      type: string
    - description: Account password
      name: password
      required: true
      type: string
    response_field: data.token
  type: http
slug: klasha-authentication
source_filename: klasha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.klasha.com/overview/authentication\ndocs: https://developers.klasha.com/overview/authentication\nnotes: >-\n  Klasha publishes no OpenAPI, so this profile is read from the documented authentication\n  page rather than derived from securitySchemes. Klasha uses a two-part scheme: a merchant\n  public key sent in the `x-auth-token` header, plus a bearer JWT obtained from a login\n  endpoint. Most privileged endpoints (payout, swap, wallet, virtual accounts) require\n  both headers together.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\nschemes:\n- name: MerchantPublicKey\n  type: apiKey\n  in: header\n  parameter_name: x-auth-token\n  description: >-\n    Merchant public key, generated from the Klasha dashboard under\n    Settings -> Generate API Keys -> Merchant public key. Sent as the value of the\n    `x-auth-token` request header\
  \ on every endpoint that requires it.\n  obtain: https://dashboard.klasha.com/settings/keys\n  source: https://developers.klasha.com/overview/authentication\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Bearer token used as the value of the `Authorization` header. Issued by the account\n    login endpoint in exchange for the account email (`username`) and `password`.\n  token_endpoint:\n    method: POST\n    path: /auth/account/v2/login\n    base: '{{env_url}}'\n    request_fields:\n    - {name: username, type: string, required: true, description: Your account email}\n    - {name: password, type: string, required: true, description: Account password}\n    response_field: data.token\n  source: https://developers.klasha.com/overview/authentication\ncombined_usage:\n  description: >-\n    Payout, swap, wallet-balance, virtual-account and webhook-resend requests are documented\n    with all three headers set together.\n  headers:\n  - {name:\
  \ Content-Type, value: application/json}\n  - {name: x-auth-token, value: merchant public key}\n  - {name: Authorization, value: 'Bearer {{token}}'}\npayload_encryption:\n  required_for: [payout, momo payout, swap]\n  algorithm: Triple-DES (3DES)\n  mode: CBC\n  padding: PKCS5Padding\n  encoding: Base64\n  envelope_field: message\n  description: >-\n    Transfer and swap request payloads must be encrypted before submission and sent as\n    a single `message` field containing the Base64 ciphertext.\n  source: https://developers.klasha.com/transfers/payout\nauth_errors:\n- {status: 400, message: public key is required}\n- {status: 400, message: Authorization required}\n- {status: 400, message: 'Invalid email or password.', error: wrong login details}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klasha/refs/heads/main/authentication/klasha-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Payments
- Cross-Border Payments
- Africa
- Emerging Markets
- Mobile Money
- Payouts
- Foreign Exchange
- Virtual Accounts
- Checkout
- Financial Services
---
