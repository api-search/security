---
api_key_in: []
api_specs:
- filename: monnify-authentication-api-openapi.yml
  format: yaml
  label: Monnify Authentication API
  slug: monnify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-authentication-api-openapi.yml
- filename: monnify-collections-api-openapi.yml
  format: yaml
  label: Monnify Collections API
  slug: monnify-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-collections-api-openapi.yml
- filename: monnify-reserved-accounts-api-openapi.yml
  format: yaml
  label: Monnify Reserved Accounts API
  slug: monnify-reserved-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-reserved-accounts-api-openapi.yml
- filename: monnify-disbursements-api-openapi.yml
  format: yaml
  label: Monnify Disbursements API
  slug: monnify-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-disbursements-api-openapi.yml
- filename: monnify-sub-accounts-api-openapi.yml
  format: yaml
  label: Monnify Sub-Accounts API
  slug: monnify-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-sub-accounts-api-openapi.yml
- filename: monnify-direct-debit-api-openapi.yml
  format: yaml
  label: Monnify Direct Debit API
  slug: monnify-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-direct-debit-api-openapi.yml
- filename: monnify-invoices-api-openapi.yml
  format: yaml
  label: Monnify Invoices API
  slug: monnify-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-invoices-api-openapi.yml
- filename: monnify-bills-payment-api-openapi.yml
  format: yaml
  label: Monnify Bills Payment API
  slug: monnify-bills-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-bills-payment-api-openapi.yml
- filename: monnify-verification-api-openapi.yml
  format: yaml
  label: Monnify Verification API
  slug: monnify-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-verification-api-openapi.yml
- filename: monnify-wallets-api-openapi.yml
  format: yaml
  label: Monnify Wallets API
  slug: monnify-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-wallets-api-openapi.yml
- filename: monnify-refunds-api-openapi.yml
  format: yaml
  label: Monnify Refunds API
  slug: monnify-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-refunds-api-openapi.yml
- filename: monnify-settlements-api-openapi.yml
  format: yaml
  label: Monnify Settlements API
  slug: monnify-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-settlements-api-openapi.yml
- filename: moniepoint-pos-api-openapi.yml
  format: yaml
  label: Moniepoint POS Push Payment API
  slug: moniepoint-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-pos-api-openapi.yml
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
- Collections
- Disbursements
- Virtual Accounts
- Direct Debit
- Bills Payment
- SMB
- Working Capital
- Unicorn
---
