---
api_key_in: []
api_specs:
- filename: doku-openapi.yml
  format: yaml
  label: DOKU Checkout API
  slug: doku-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Access Token API
  slug: doku-snap-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Virtual Account API
  slug: doku-snap-virtual-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Direct Debit & e-Wallet API
  slug: doku-snap-direct-debit-ewallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP QRIS API
  slug: doku-snap-qris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU Kirim Payout API
  slug: doku-kirim-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Doku Authentication
name_suffix: Authentication
oauth_flows: []
overview: DOKU secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DOKU
provider_slug: doku
scheme_count: 4
schemes:
- algorithm: HMAC-SHA256
  companionHeaders:
  - Client-Id
  - Request-Id
  - Request-Timestamp
  componentString: Client-Id:<v>\nRequest-Id:<v>\nRequest-Timestamp:<v>\nRequest-Target:<path>\nDigest:<sha256-of-body>
  format: 'Signature: HMACSHA256=<base64(hmacSha256(clientSecret, componentString))>'
  headerName: Signature
  in: header
  name: checkout_signature
  scope: DOKU Checkout API and legacy non-SNAP Direct API
  sources:
  - https://developers.doku.com/accept-payments/doku-checkout/integration-guide/backend-integration
  type: apiKey
- algorithm: SHA256withRSA (asymmetric)
  companionHeaders:
  - X-CLIENT-KEY
  - X-TIMESTAMP
  endpoint: POST /authorization/v1/access-token/b2b
  headerName: X-SIGNATURE
  in: header
  name: snap_asymmetric_token
  scope: SNAP access-token issuance (B2B and B2B2C)
  sources:
  - https://developers.doku.com/accept-payments/direct-api/snap/integration-guide/get-token-api/b2b
  stringToSign: <clientId>|<X-TIMESTAMP>
  tokenTtlSeconds: 900
  type: apiKey
- bearerFormat: JWT
  headerName: Authorization
  name: snap_bearer
  scheme: bearer
  scope: All SNAP transaction endpoints (Virtual Account, Direct Debit / e-Wallet, QRIS, Kirim payout)
  sources:
  - https://developers.doku.com/accept-payments/direct-api/snap/integration-guide/get-token-api/b2b
  type: http
- algorithm: HMAC-SHA512 (symmetric)
  companionHeaders:
  - X-PARTNER-ID
  - X-EXTERNAL-ID
  - X-TIMESTAMP
  - CHANNEL-ID
  headerName: X-SIGNATURE
  in: header
  name: snap_symmetric_signature
  scope: SNAP transaction signing per request
  sources:
  - https://developers.doku.com/accept-payments/direct-api/snap/integration-guide/virtual-account/bca-virtual-account
  stringToSign: <HTTPMethod>:<EndpointUrl>:<AccessToken>:Lowercase(HexEncode(SHA-256(minified-body))):<X-TIMESTAMP>
  type: apiKey
slug: doku-authentication
source_filename: doku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\ndocs: https://developers.doku.com/accept-payments/direct-api/snap/integration-guide/get-token-api/b2b\nsource: openapi/doku-openapi.yml + developers.doku.com\nsummary:\n  types:\n  - apiKey\n  - http\n  notes: >-\n    DOKU runs two distinct request-signing models. (1) Non-SNAP (Checkout and\n    legacy Direct API): request-level HMAC-SHA256 signature carried in a\n    Signature header alongside Client-Id, Request-Id, and Request-Timestamp.\n    (2) Bank Indonesia SNAP: an asymmetric SHA256withRSA signature to obtain a\n    15-minute Bearer access token, then a symmetric HMAC-SHA512 signature per\n    transaction. No credentials are ever placed in the URL; all traffic is\n    HTTPS/TLS to region hosts.\nschemes:\n- name: checkout_signature\n  type: apiKey\n  in: header\n  headerName: Signature\n  companionHeaders:\n  - Client-Id\n  - Request-Id\n  - Request-Timestamp\n  algorithm: HMAC-SHA256\n  format: 'Signature: HMACSHA256=<base64(hmacSha256(clientSecret,\
  \ componentString))>'\n  componentString: >-\n    Client-Id:<v>\\nRequest-Id:<v>\\nRequest-Timestamp:<v>\\nRequest-Target:<path>\\nDigest:<sha256-of-body>\n  scope: DOKU Checkout API and legacy non-SNAP Direct API\n  sources:\n  - https://developers.doku.com/accept-payments/doku-checkout/integration-guide/backend-integration\n- name: snap_asymmetric_token\n  type: apiKey\n  in: header\n  headerName: X-SIGNATURE\n  companionHeaders:\n  - X-CLIENT-KEY\n  - X-TIMESTAMP\n  algorithm: SHA256withRSA (asymmetric)\n  stringToSign: '<clientId>|<X-TIMESTAMP>'\n  endpoint: POST /authorization/v1/access-token/b2b\n  scope: SNAP access-token issuance (B2B and B2B2C)\n  tokenTtlSeconds: 900\n  sources:\n  - https://developers.doku.com/accept-payments/direct-api/snap/integration-guide/get-token-api/b2b\n- name: snap_bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  headerName: Authorization\n  scope: All SNAP transaction endpoints (Virtual Account, Direct Debit / e-Wallet, QRIS, Kirim payout)\n\
  \  sources:\n  - https://developers.doku.com/accept-payments/direct-api/snap/integration-guide/get-token-api/b2b\n- name: snap_symmetric_signature\n  type: apiKey\n  in: header\n  headerName: X-SIGNATURE\n  companionHeaders:\n  - X-PARTNER-ID\n  - X-EXTERNAL-ID\n  - X-TIMESTAMP\n  - CHANNEL-ID\n  algorithm: HMAC-SHA512 (symmetric)\n  stringToSign: >-\n    <HTTPMethod>:<EndpointUrl>:<AccessToken>:Lowercase(HexEncode(SHA-256(minified-body))):<X-TIMESTAMP>\n  scope: SNAP transaction signing per request\n  sources:\n  - https://developers.doku.com/accept-payments/direct-api/snap/integration-guide/virtual-account/bca-virtual-account\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/authentication/doku-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Payments
- Payment Gateway
- Fintech
- Indonesia
- SEA
- SNAP
- Virtual Account
- E-Wallet
- QRIS
- Direct Debit
- Payouts
---
