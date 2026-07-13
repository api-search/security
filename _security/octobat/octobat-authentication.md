---
api_key_in: []
api_specs:
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Invoices API
  slug: octobat-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Credit Notes API
  slug: octobat-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Transactions API
  slug: octobat-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Customers API
  slug: octobat-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Products API
  slug: octobat-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Tax Evidence API
  slug: octobat-tax-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Coupons API
  slug: octobat-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Subscriptions API
  slug: octobat-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
- filename: octobat-openapi.yml
  format: yaml
  label: Octobat Payouts API
  slug: octobat-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/openapi/octobat-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Octobat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octobat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Octobat
provider_slug: octobat
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. Use your Octobat secret key as the username and leave the password empty (curl: -u sk_live_xxx:). Use sk_test_ keys for test mode and sk_live_ keys for live mode.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/octobat-openapi.yml
  type: http
slug: octobat-authentication
source_filename: octobat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/octobat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic authentication. Use your Octobat secret key as the username and leave\n    the password empty (curl: -u sk_live_xxx:). Use sk_test_ keys for test mode and sk_live_\n    keys for live mode.'\n  sources:\n  - openapi/octobat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octobat/refs/heads/main/authentication/octobat-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Invoicing
- Tax Compliance
- VAT
- E-Commerce
- Payments
- Fintech
---
