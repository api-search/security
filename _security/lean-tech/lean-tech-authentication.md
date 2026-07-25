---
api_key_in: []
api_specs:
- filename: lean-tech-account-on-file-api-openapi.yml
  format: yaml
  label: Lean Technologies Account on File API
  slug: lean-tech-account-on-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-account-on-file-api-openapi.yml
- filename: lean-tech-account-verification-api-openapi.yml
  format: yaml
  label: Lean Technologies Account Verification API
  slug: lean-tech-account-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-account-verification-api-openapi.yml
- filename: lean-tech-accounts-api-openapi.yml
  format: yaml
  label: Lean Technologies Accounts API
  slug: lean-tech-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-accounts-api-openapi.yml
- filename: lean-tech-authentication-api-openapi.yml
  format: yaml
  label: Lean Technologies Authentication API
  slug: lean-tech-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-authentication-api-openapi.yml
- filename: lean-tech-balances-api-openapi.yml
  format: yaml
  label: Lean Technologies Balances API
  slug: lean-tech-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-balances-api-openapi.yml
- filename: lean-tech-banks-api-openapi.yml
  format: yaml
  label: Lean Technologies Banks API
  slug: lean-tech-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-banks-api-openapi.yml
- filename: lean-tech-consents-api-openapi.yml
  format: yaml
  label: Lean Technologies Consents API
  slug: lean-tech-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-consents-api-openapi.yml
- filename: lean-tech-customers-api-openapi.yml
  format: yaml
  label: Lean Technologies Customers API
  slug: lean-tech-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-customers-api-openapi.yml
- filename: lean-tech-entities-api-openapi.yml
  format: yaml
  label: Lean Technologies Entities API
  slug: lean-tech-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-entities-api-openapi.yml
- filename: lean-tech-identity-api-openapi.yml
  format: yaml
  label: Lean Technologies Identity API
  slug: lean-tech-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-identity-api-openapi.yml
- filename: lean-tech-insights-api-openapi.yml
  format: yaml
  label: Lean Technologies Insights API
  slug: lean-tech-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-insights-api-openapi.yml
- filename: lean-tech-name-verification-api-openapi.yml
  format: yaml
  label: Lean Technologies Name Verification API
  slug: lean-tech-name-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-name-verification-api-openapi.yml
- filename: lean-tech-payment-intents-api-openapi.yml
  format: yaml
  label: Lean Technologies Payment Intents API
  slug: lean-tech-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-payment-intents-api-openapi.yml
- filename: lean-tech-payment-sources-api-openapi.yml
  format: yaml
  label: Lean Technologies Payment Sources API
  slug: lean-tech-payment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-payment-sources-api-openapi.yml
- filename: lean-tech-payout-destinations-api-openapi.yml
  format: yaml
  label: Lean Technologies Payout Destinations API
  slug: lean-tech-payout-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-payout-destinations-api-openapi.yml
- filename: lean-tech-payouts-api-openapi.yml
  format: yaml
  label: Lean Technologies Payouts API
  slug: lean-tech-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-payouts-api-openapi.yml
- filename: lean-tech-refreshes-api-openapi.yml
  format: yaml
  label: Lean Technologies Refreshes API
  slug: lean-tech-refreshes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-refreshes-api-openapi.yml
- filename: lean-tech-refunds-api-openapi.yml
  format: yaml
  label: Lean Technologies Refunds API
  slug: lean-tech-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-refunds-api-openapi.yml
- filename: lean-tech-transactions-api-openapi.yml
  format: yaml
  label: Lean Technologies Transactions API
  slug: lean-tech-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-tech-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lean Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lean Technologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lean Technologies
provider_slug: lean-tech
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lean-banks-api-openapi.yml
  - openapi/lean-customers-api-openapi.yml
  - openapi/lean-data-api-openapi.yml
  - openapi/lean-entities-api-openapi.yml
  - openapi/lean-insights-api-openapi.yml
  - openapi/lean-payment-sources-api-openapi.yml
  - openapi/lean-payments-api-openapi.yml
  - openapi/lean-payouts-api-openapi.yml
  - openapi/lean-refunds-api-openapi.yml
  - openapi/lean-verifications-api-openapi.yml
  type: http
slug: lean-tech-authentication
source_filename: lean-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lean-banks-api-openapi.yml, openapi/lean-customers-api-openapi.yml, openapi/lean-data-api-openapi.yml,\n  openapi/lean-entities-api-openapi.yml, openapi/lean-insights-api-openapi.yml, openapi/lean-payment-sources-api-openapi.yml,\n  openapi/lean-payments-api-openapi.yml, openapi/lean-payouts-api-openapi.yml, openapi/lean-refunds-api-openapi.yml,\n  openapi/lean-verifications-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lean-banks-api-openapi.yml\n  - openapi/lean-customers-api-openapi.yml\n  - openapi/lean-data-api-openapi.yml\n  - openapi/lean-entities-api-openapi.yml\n  - openapi/lean-insights-api-openapi.yml\n  - openapi/lean-payment-sources-api-openapi.yml\n  - openapi/lean-payments-api-openapi.yml\n  - openapi/lean-payouts-api-openapi.yml\n  - openapi/lean-refunds-api-openapi.yml\n  - openapi/lean-verifications-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/authentication/lean-tech-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- Open Finance
- MENA
- UAE
- Saudi Arabia
- Payments
- Pay by Bank
- A2A
- Account Information
- Payment Initiation
- Verifications
- Identity
- Fintech
---
