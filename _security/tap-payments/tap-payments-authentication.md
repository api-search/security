---
api_key_in: []
api_specs:
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Charges API
  slug: tap-payments-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Authorize API
  slug: tap-payments-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Refunds API
  slug: tap-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Customers API
  slug: tap-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Tokens API
  slug: tap-payments-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Cards API
  slug: tap-payments-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Invoices API
  slug: tap-payments-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Payouts API
  slug: tap-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Business API
  slug: tap-payments-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tap Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tap Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tap Payments
provider_slug: tap-payments
scheme_count: 1
schemes:
- description: 'Secret API key passed as a Bearer token: `Authorization: Bearer sk_test_...` (test) or `Authorization: Bearer sk_live_...` (live). Keys are issued from the Tap dashboard, with separate keys per mode. The secret key must remain server-side; a publishable key (pk_test_ / pk_live_) is used for client-side tokenization only.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tap-payments-openapi.yml
  - https://developers.tap.company/reference/api-endpoint
  type: http
slug: tap-payments-authentication
source_filename: tap-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/tap-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Secret API key passed as a Bearer token: `Authorization: Bearer sk_test_...`\n    (test) or `Authorization: Bearer sk_live_...` (live). Keys are issued from the\n    Tap dashboard, with separate keys per mode. The secret key must remain\n    server-side; a publishable key (pk_test_ / pk_live_) is used for client-side\n    tokenization only.'\n  sources:\n  - openapi/tap-payments-openapi.yml\n  - https://developers.tap.company/reference/api-endpoint\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/authentication/tap-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Fintech
- Payment Gateway
- MENA
- Middle East
- Online Payments
- Charges
- Cards
- KNET
- mada
- Financial Infrastructure
---
