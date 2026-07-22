---
api_key_in:
- header
- query
auth_types:
- apiKey
- http-bearer
- request-signing
description: ''
kind: authentication
layout: security
method: searched
name: Moonpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoonPay secures its APIs with apiKey, http-bearer, and request-signing across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MoonPay
provider_slug: moonpay
scheme_count: 4
schemes:
- docs: https://dev.moonpay.com/platform/guides/api-and-sdk-credentials
  in: header
  name: SecretKeyHeader
  parameter: X-Api-Key
  scope: server-side
  type: apiKey
  usage: Server-to-server requests. Test key prefix sk_test_, live key prefix sk_live_.
- in: query
  name: ApiKeyQuery
  parameter: apiKey
  scope: client-side
  type: apiKey
  usage: Publishable key used to initialize widget/client requests.
- name: AccessTokenBearer
  scheme: bearer
  scope: client-side
  token_lifetime: short-lived (expiresAt on issued credentials)
  type: http
  usage: 'Client-side Platform API requests use the accessToken returned from a connection as a Bearer token (Authorization: Bearer <accessToken>).'
- algorithm: HMAC-SHA256
  docs: https://dev.moonpay.com/api-reference/widget/webhooks/signature
  name: WidgetUrlSignature
  type: request-signing
  usage: Widget/checkout URLs and certain requests are signed with the account secret key; webhooks are verified with a request signature (see webhooks/signature docs).
slug: moonpay-authentication
source_filename: moonpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://dev.moonpay.com/api-reference/platform/documentation/using-the-api\ndocs: https://dev.moonpay.com/platform/guides/api-and-sdk-credentials\nsummary:\n  types: [apiKey, http-bearer, request-signing]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n  - name: SecretKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-Api-Key\n    usage: Server-to-server requests. Test key prefix sk_test_, live key prefix sk_live_.\n    scope: server-side\n    docs: https://dev.moonpay.com/platform/guides/api-and-sdk-credentials\n  - name: ApiKeyQuery\n    type: apiKey\n    in: query\n    parameter: apiKey\n    usage: Publishable key used to initialize widget/client requests.\n    scope: client-side\n  - name: AccessTokenBearer\n    type: http\n    scheme: bearer\n    usage: >-\n      Client-side Platform API requests use the accessToken returned from a connection\n      as a Bearer token (Authorization: Bearer <accessToken>).\n\
  \    scope: client-side\n    token_lifetime: short-lived (expiresAt on issued credentials)\n  - name: WidgetUrlSignature\n    type: request-signing\n    algorithm: HMAC-SHA256\n    usage: >-\n      Widget/checkout URLs and certain requests are signed with the account secret key;\n      webhooks are verified with a request signature (see webhooks/signature docs).\n    docs: https://dev.moonpay.com/api-reference/widget/webhooks/signature\nnotes:\n  - Test vs live mode is selected by the key prefix (sk_test_/sk_live_), not the URL.\n  - Secret keys must never be exposed to the frontend; client flows use short-lived accessTokens.\n  - No OAuth2/OIDC scope surface is documented; auth is key + bearer-token based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonpay/refs/heads/main/authentication/moonpay-authentication.yml
summary_line: apiKey/http-bearer/request-signing · 4 schemes
tags:
- Company
- Crypto Infrastructure
- Payments
- Cryptocurrency
- On-Ramp
- Off-Ramp
- Fintech
- Digital Wallet
- Blockchain
- KYC
---
