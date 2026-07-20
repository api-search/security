---
api_key_in: []
api_specs:
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Charges API
  slug: payjp-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Customers API
  slug: payjp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Cards API
  slug: payjp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Tokens API
  slug: payjp-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Plans API
  slug: payjp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Subscriptions API
  slug: payjp-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Transfers API
  slug: payjp-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Statements & Balances API
  slug: payjp-statements-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Events & Webhooks API
  slug: payjp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP 3D Secure API
  slug: payjp-three-d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Platform API (Tenants)
  slug: payjp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Account API
  slug: payjp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Payjp Authentication
name_suffix: Authentication
oauth_flows: []
overview: PAY.JP secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PAY.JP
provider_slug: payjp
scheme_count: 2
schemes:
- in: header
  keyPrefixes:
  - sk_test_
  - sk_live_
  name: secret_key
  note: Secret key as Basic username, empty password. Server-side only; never expose.
  scheme: basic
  sources:
  - openapi/payjp-openapi.yml
  - https://docs.pay.jp/v1/api/
  type: http
- in: body
  keyPrefixes:
  - pk_test_
  - pk_live_
  name: publishable_key
  note: Publishable key used client-side by payjp.js / Checkout to create single-use card tokens (POST /tokens). Safe to embed in front-end code; cannot read or charge.
  sources:
  - https://docs.pay.jp/v1/api/
  type: apiKey
slug: payjp-authentication
source_filename: payjp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/payjp-openapi.yml\nnotes: >-\n  PAY.JP authenticates REST requests with HTTP Basic auth: the secret key\n  (sk_test_ / sk_live_) is sent as the Basic username with an empty password.\n  Client-side tokenization (payjp.js / Checkout) uses the publishable key\n  (pk_test_ / pk_live_) instead, which can only create tokens.\nsummary:\n  types:\n  - http\nschemes:\n- name: secret_key\n  type: http\n  scheme: basic\n  in: header\n  keyPrefixes:\n  - sk_test_\n  - sk_live_\n  note: Secret key as Basic username, empty password. Server-side only; never expose.\n  sources:\n  - openapi/payjp-openapi.yml\n  - https://docs.pay.jp/v1/api/\n- name: publishable_key\n  type: apiKey\n  in: body\n  keyPrefixes:\n  - pk_test_\n  - pk_live_\n  note: >-\n    Publishable key used client-side by payjp.js / Checkout to create single-use\n    card tokens (POST /tokens). Safe to embed in front-end code; cannot read or\n    charge.\n  sources:\n\
  \  - https://docs.pay.jp/v1/api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/authentication/payjp-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- FinTech
- Japan
- Credit Cards
- Subscriptions
- Tokenization
---
