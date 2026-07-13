---
api_key_in: []
api_specs:
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Payments API
  slug: toss-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Billing API
  slug: toss-payments-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Virtual Accounts API
  slug: toss-payments-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Cash Receipts API
  slug: toss-payments-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Transactions API
  slug: toss-payments-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Settlements API
  slug: toss-payments-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Payouts API
  slug: toss-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Toss Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toss Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Toss Payments
provider_slug: toss-payments
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication using a Toss Payments secret API key. The secret key is used as the username with an empty password, then Base64 encoded: `Authorization: Basic base64(secretKey:)` (note the trailing colon). Test secret keys are prefixed `test_sk_` / `test_gsk_`; live secret keys are prefixed `live_sk_` / `live_gsk_`. Browser-side client keys (`test_ck_` / `live_ck_`) are used by the JavaScript SDK / payment widget and do not authenticate Core API calls.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/toss-payments-openapi.yml
  - https://docs.tosspayments.com/en/api-guide
  type: http
slug: toss-payments-authentication
source_filename: toss-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/toss-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication using a Toss Payments secret API key. The secret\n    key is used as the username with an empty password, then Base64 encoded:\n    `Authorization: Basic base64(secretKey:)` (note the trailing colon). Test\n    secret keys are prefixed `test_sk_` / `test_gsk_`; live secret keys are\n    prefixed `live_sk_` / `live_gsk_`. Browser-side client keys (`test_ck_` /\n    `live_ck_`) are used by the JavaScript SDK / payment widget and do not\n    authenticate Core API calls.\n  sources:\n  - openapi/toss-payments-openapi.yml\n  - https://docs.tosspayments.com/en/api-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/authentication/toss-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- South Korea
- Cards
- Easy Pay
- Virtual Account
- Billing
- Checkout
- Fintech
---
