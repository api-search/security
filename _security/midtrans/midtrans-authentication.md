---
api_key_in: []
api_specs:
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Snap API
  slug: midtrans-snap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Core API
  slug: midtrans-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Card Tokenization API
  slug: midtrans-card-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans GoPay Tokenization API
  slug: midtrans-gopay-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Payment Link API
  slug: midtrans-payment-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Subscription API
  slug: midtrans-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Iris Disbursement API
  slug: midtrans-iris-disbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Midtrans Authentication
name_suffix: Authentication
oauth_flows: []
overview: Midtrans secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Midtrans
provider_slug: midtrans
scheme_count: 3
schemes:
- description: 'HTTP Basic authentication for all server-to-server calls (Snap, Core API charge and lifecycle, Payment Link, Subscription). The Server Key is the username and the password is empty, so the header is `Authorization: Basic base64(SERVER_KEY:)`. Server Keys are issued per environment in the Midtrans dashboard; Sandbox keys are prefixed `SB-Mid-server-`.'
  name: serverKeyAuth
  scheme: basic
  sources:
  - openapi/midtrans-openapi.yml
  - https://docs.midtrans.com/docs/api-authorization-headers
  type: http
- description: Public Client Key passed as the `client_key` query parameter on the browser-side card tokenization endpoints (`GET /v2/token`, `GET /v2/card/register`). Being public, it can only mint one-time card tokens - it cannot charge or read transactions. Sandbox keys are prefixed `SB-Mid-client-`.
  in: query
  name: clientKeyQuery
  parameterName: client_key
  sources:
  - openapi/midtrans-openapi.yml
  - https://docs.midtrans.com/reference/get-token
  type: apiKey
- description: Iris disbursement uses its own creator / approver API key over HTTP Basic (key as username, empty password), separate from the payment Server Key. Sensitive payout approval can additionally require an OTP.
  name: irisApiKey
  scheme: basic
  sources:
  - https://docs.midtrans.com/docs/disbursement-overview
  type: http
slug: midtrans-authentication
source_filename: midtrans-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/midtrans-openapi.yml\nsummary:\n  types:\n  - http\n  - apiKey\nschemes:\n- name: serverKeyAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication for all server-to-server calls (Snap, Core API\n    charge and lifecycle, Payment Link, Subscription). The Server Key is the\n    username and the password is empty, so the header is\n    `Authorization: Basic base64(SERVER_KEY:)`. Server Keys are issued per\n    environment in the Midtrans dashboard; Sandbox keys are prefixed\n    `SB-Mid-server-`.\n  sources:\n  - openapi/midtrans-openapi.yml\n  - https://docs.midtrans.com/docs/api-authorization-headers\n- name: clientKeyQuery\n  type: apiKey\n  in: query\n  parameterName: client_key\n  description: >-\n    Public Client Key passed as the `client_key` query parameter on the\n    browser-side card tokenization endpoints (`GET /v2/token`,\n    `GET /v2/card/register`). Being public, it can only\
  \ mint one-time card\n    tokens - it cannot charge or read transactions. Sandbox keys are prefixed\n    `SB-Mid-client-`.\n  sources:\n  - openapi/midtrans-openapi.yml\n  - https://docs.midtrans.com/reference/get-token\n- name: irisApiKey\n  type: http\n  scheme: basic\n  description: >-\n    Iris disbursement uses its own creator / approver API key over HTTP Basic\n    (key as username, empty password), separate from the payment Server Key.\n    Sensitive payout approval can additionally require an OTP.\n  sources:\n  - https://docs.midtrans.com/docs/disbursement-overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/authentication/midtrans-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Payments
- Payment Gateway
- Indonesia
- Southeast Asia
- Snap
- E-Wallet
- Virtual Account
- Cards
- Bank Transfer
- Fintech
---
