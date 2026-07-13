---
api_key_in: []
api_specs:
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payment Requests API
  slug: xendit-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payment Tokens API
  slug: xendit-payment-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Invoices API
  slug: xendit-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payouts API
  slug: xendit-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Balance API
  slug: xendit-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Transactions API
  slug: xendit-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Customers API
  slug: xendit-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Refunds API
  slug: xendit-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Xendit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xendit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xendit
provider_slug: xendit
scheme_count: 1
schemes:
- description: HTTP Basic Access Authentication. Use your Xendit secret API key as the username and leave the password empty; the client Base64-encodes "SECRET_KEY:" into the Authorization header. Secret keys are issued self-serve from the Xendit dashboard in both test mode and (after business verification) live mode. An optional `for-user-id` header targets a xenPlatform sub-account, and the v3 Payments API additionally requires an `api-version` header (2024-11-11).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/xendit-openapi.yml
  - https://docs.xendit.co/apidocs/quick-setup
  type: http
slug: xendit-authentication
source_filename: xendit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/xendit-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic Access Authentication. Use your Xendit secret API key as the\n    username and leave the password empty; the client Base64-encodes\n    \"SECRET_KEY:\" into the Authorization header. Secret keys are issued\n    self-serve from the Xendit dashboard in both test mode and (after business\n    verification) live mode. An optional `for-user-id` header targets a\n    xenPlatform sub-account, and the v3 Payments API additionally requires an\n    `api-version` header (2024-11-11).\n  sources:\n  - openapi/xendit-openapi.yml\n  - https://docs.xendit.co/apidocs/quick-setup\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/authentication/xendit-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Fintech
- Payment Gateway
- Southeast Asia
- Indonesia
- Philippines
- Disbursements
- E-Wallet
- Virtual Accounts
- Cards
- Financial Infrastructure
---
