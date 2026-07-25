---
api_key_in: []
api_specs:
- filename: resolve-access-keys-api-openapi.yml
  format: yaml
  label: Resolve Access Keys API
  slug: resolve-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-access-keys-api-openapi.yml
- filename: resolve-charges-api-openapi.yml
  format: yaml
  label: Resolve Charges API
  slug: resolve-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-charges-api-openapi.yml
- filename: resolve-credit-notes-api-openapi.yml
  format: yaml
  label: Resolve Credit Notes API
  slug: resolve-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-credit-notes-api-openapi.yml
- filename: resolve-customers-api-openapi.yml
  format: yaml
  label: Resolve Customers API
  slug: resolve-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-customers-api-openapi.yml
- filename: resolve-invoices-api-openapi.yml
  format: yaml
  label: Resolve Invoices API
  slug: resolve-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-invoices-api-openapi.yml
- filename: resolve-merchants-api-openapi.yml
  format: yaml
  label: Resolve Merchants API
  slug: resolve-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-merchants-api-openapi.yml
- filename: resolve-orders-api-openapi.yml
  format: yaml
  label: Resolve Orders API
  slug: resolve-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-orders-api-openapi.yml
- filename: resolve-payments-api-openapi.yml
  format: yaml
  label: Resolve Payments API
  slug: resolve-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-payments-api-openapi.yml
- filename: resolve-payout-transactions-api-openapi.yml
  format: yaml
  label: Resolve Payout Transactions API
  slug: resolve-payout-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-payout-transactions-api-openapi.yml
- filename: resolve-payouts-api-openapi.yml
  format: yaml
  label: Resolve Payouts API
  slug: resolve-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-payouts-api-openapi.yml
- filename: resolve-shipments-api-openapi.yml
  format: yaml
  label: Resolve Shipments API
  slug: resolve-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-shipments-api-openapi.yml
- filename: resolve-webhooks-api-openapi.yml
  format: yaml
  label: Resolve Webhooks API
  slug: resolve-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Resolve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Resolve secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Resolve
provider_slug: resolve
scheme_count: 2
schemes:
- description: HTTP Basic Auth using `merchant_id` as username and the merchant secret key as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/resolve-merchant-api-openapi.yaml
  - openapi/resolve-partners-api-openapi.yaml
  type: http
- bearerFormat: JWT
  description: Bearer token authentication using an OAuth access token minted for an API access key created in Merchant Dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/resolve-merchant-api-openapi.yaml
  - openapi/resolve-partners-api-openapi.yaml
  type: http
slug: resolve-authentication
source_filename: resolve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/resolve-merchant-api-openapi.yaml, openapi/resolve-partners-api-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using `merchant_id` as username and the merchant secret key as\n    password.\n  sources:\n  - openapi/resolve-merchant-api-openapi.yaml\n  - openapi/resolve-partners-api-openapi.yaml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication using an OAuth access token minted for an API access\n    key created in Merchant Dashboard.\n  sources:\n  - openapi/resolve-merchant-api-openapi.yaml\n  - openapi/resolve-partners-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/authentication/resolve-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Payments
- B2B
- Net Terms
- Credit
- Invoicing
- Financing
- Embedded Finance
---
