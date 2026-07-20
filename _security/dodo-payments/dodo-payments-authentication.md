---
api_key_in: []
api_specs:
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Products API
  slug: dodo-payments-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Payments API
  slug: dodo-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Subscriptions API
  slug: dodo-payments-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Customers API
  slug: dodo-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Checkout Sessions API
  slug: dodo-payments-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Discounts API
  slug: dodo-payments-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Licenses API
  slug: dodo-payments-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Payouts API
  slug: dodo-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Webhooks API
  slug: dodo-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dodo Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dodo Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dodo Payments
provider_slug: dodo-payments
scheme_count: 1
schemes:
- description: 'Authenticate with your Dodo Payments API key as a bearer token: `Authorization: Bearer [example key]`. Use a test-mode key against https://test.dodopayments.com and a live-mode key against https://live.dodopayments.com.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dodo-payments-openapi.yml
  type: http
slug: dodo-payments-authentication
source_filename: dodo-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dodo-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate with your Dodo Payments API key as a bearer token: `Authorization:\n    Bearer [example key]`. Use a test-mode key against https://test.dodopayments.com and a live-mode\n    key against https://live.dodopayments.com.'\n  sources:\n  - openapi/dodo-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/authentication/dodo-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Merchant of Record
- Subscriptions
- Billing
- Global Commerce
---
