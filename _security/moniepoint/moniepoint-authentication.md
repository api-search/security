---
api_key_in: []
api_specs:
- filename: moniepoint-authentication-api-openapi.yml
  format: yaml
  label: Moniepoint Authentication API
  slug: moniepoint-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-authentication-api-openapi.yml
- filename: moniepoint-banks-api-openapi.yml
  format: yaml
  label: Moniepoint Banks API
  slug: moniepoint-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-banks-api-openapi.yml
- filename: moniepoint-bills-payment-api-openapi.yml
  format: yaml
  label: Moniepoint Bills Payment API
  slug: moniepoint-bills-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-bills-payment-api-openapi.yml
- filename: moniepoint-bulk-transfers-api-openapi.yml
  format: yaml
  label: Moniepoint Bulk Transfers API
  slug: moniepoint-bulk-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-bulk-transfers-api-openapi.yml
- filename: moniepoint-debits-api-openapi.yml
  format: yaml
  label: Moniepoint Debits API
  slug: moniepoint-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-debits-api-openapi.yml
- filename: moniepoint-invoices-api-openapi.yml
  format: yaml
  label: Moniepoint Invoices API
  slug: moniepoint-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-invoices-api-openapi.yml
- filename: moniepoint-limit-profiles-api-openapi.yml
  format: yaml
  label: Moniepoint Limit Profiles API
  slug: moniepoint-limit-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-limit-profiles-api-openapi.yml
- filename: moniepoint-mandates-api-openapi.yml
  format: yaml
  label: Moniepoint Mandates API
  slug: moniepoint-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-mandates-api-openapi.yml
- filename: moniepoint-push-payments-api-openapi.yml
  format: yaml
  label: Moniepoint Push Payments API
  slug: moniepoint-push-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-push-payments-api-openapi.yml
- filename: moniepoint-refunds-api-openapi.yml
  format: yaml
  label: Moniepoint Refunds API
  slug: moniepoint-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-refunds-api-openapi.yml
- filename: moniepoint-reserved-accounts-api-openapi.yml
  format: yaml
  label: Moniepoint Reserved Accounts API
  slug: moniepoint-reserved-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-reserved-accounts-api-openapi.yml
- filename: moniepoint-settlements-api-openapi.yml
  format: yaml
  label: Moniepoint Settlements API
  slug: moniepoint-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-settlements-api-openapi.yml
- filename: moniepoint-single-transfers-api-openapi.yml
  format: yaml
  label: Moniepoint Single Transfers API
  slug: moniepoint-single-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-single-transfers-api-openapi.yml
- filename: moniepoint-sub-accounts-api-openapi.yml
  format: yaml
  label: Moniepoint Sub-Accounts API
  slug: moniepoint-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-sub-accounts-api-openapi.yml
- filename: moniepoint-transactions-api-openapi.yml
  format: yaml
  label: Moniepoint Transactions API
  slug: moniepoint-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-transactions-api-openapi.yml
- filename: moniepoint-verification-api-openapi.yml
  format: yaml
  label: Moniepoint Verification API
  slug: moniepoint-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-verification-api-openapi.yml
- filename: moniepoint-wallet-api-openapi.yml
  format: yaml
  label: Moniepoint Wallet API
  slug: moniepoint-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-wallet-api-openapi.yml
- filename: moniepoint-wallets-api-openapi.yml
  format: yaml
  label: Moniepoint Wallets API
  slug: moniepoint-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-wallets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moniepoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moniepoint secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Moniepoint
provider_slug: moniepoint
scheme_count: 2
schemes:
- description: Basic auth using API client id and client secret from the Moniepoint Business dashboard.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/moniepoint-pos-api-openapi.yml
  - openapi/monnify-authentication-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/monnify-bills-payment-api-openapi.yml
  - openapi/monnify-collections-api-openapi.yml
  - openapi/monnify-direct-debit-api-openapi.yml
  - openapi/monnify-disbursements-api-openapi.yml
  - openapi/monnify-invoices-api-openapi.yml
  - openapi/monnify-refunds-api-openapi.yml
  - openapi/monnify-reserved-accounts-api-openapi.yml
  - openapi/monnify-settlements-api-openapi.yml
  - openapi/monnify-sub-accounts-api-openapi.yml
  - openapi/monnify-verification-api-openapi.yml
  - openapi/monnify-wallets-api-openapi.yml
  type: http
slug: moniepoint-authentication
source_filename: moniepoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moniepoint-pos-api-openapi.yml, openapi/monnify-authentication-api-openapi.yml,\n  openapi/monnify-bills-payment-api-openapi.yml, openapi/monnify-collections-api-openapi.yml,\n  openapi/monnify-direct-debit-api-openapi.yml, openapi/monnify-disbursements-api-openapi.yml,\n  openapi/monnify-invoices-api-openapi.yml, openapi/monnify-refunds-api-openapi.yml, openapi/monnify-reserved-accounts-api-openapi.yml,\n  openapi/monnify-settlements-api-openapi.yml, openapi/monnify-sub-accounts-api-openapi.yml,\n  openapi/monnify-verification-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic auth using API client id and client secret from the Moniepoint Business\n    dashboard.\n  sources:\n  - openapi/moniepoint-pos-api-openapi.yml\n  - openapi/monnify-authentication-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ JWT\n  sources:\n  - openapi/monnify-bills-payment-api-openapi.yml\n  - openapi/monnify-collections-api-openapi.yml\n  - openapi/monnify-direct-debit-api-openapi.yml\n  - openapi/monnify-disbursements-api-openapi.yml\n  - openapi/monnify-invoices-api-openapi.yml\n  - openapi/monnify-refunds-api-openapi.yml\n  - openapi/monnify-reserved-accounts-api-openapi.yml\n  - openapi/monnify-settlements-api-openapi.yml\n  - openapi/monnify-sub-accounts-api-openapi.yml\n  - openapi/monnify-verification-api-openapi.yml\n  - openapi/monnify-wallets-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/authentication/moniepoint-authentication.yml
summary_line: http · 2 schemes
tags:
- Africa
- Nigeria
- Payments
- Banking
- Fintech
- Acquiring
- POS
- Collection
- Disbursements
- Virtual Accounts
- Direct Debit
- Bills Payment
- SMB
- Working Capital
- Unicorn
---
