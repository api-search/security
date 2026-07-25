---
api_key_in:
- header
api_specs:
- filename: dlocal-payouts-api-openapi.yml
  format: yaml
  label: dLocal Payouts API
  slug: dlocal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payouts-api-openapi.yml
- filename: dlocal-accounts-api-openapi.yml
  format: yaml
  label: dLocal Accounts API
  slug: dlocal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-accounts-api-openapi.yml
- filename: dlocal-balance-api-openapi.yml
  format: yaml
  label: dLocal Balance API
  slug: dlocal-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-balance-api-openapi.yml
- filename: dlocal-bank-accounts-api-openapi.yml
  format: yaml
  label: dLocal Bank Accounts API
  slug: dlocal-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-bank-accounts-api-openapi.yml
- filename: dlocal-chargebacks-api-openapi.yml
  format: yaml
  label: dLocal Chargebacks API
  slug: dlocal-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-chargebacks-api-openapi.yml
- filename: dlocal-currency-api-openapi.yml
  format: yaml
  label: dLocal Currency API
  slug: dlocal-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-currency-api-openapi.yml
- filename: dlocal-documents-api-openapi.yml
  format: yaml
  label: dLocal Documents API
  slug: dlocal-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-documents-api-openapi.yml
- filename: dlocal-kyc-api-openapi.yml
  format: yaml
  label: dLocal KYC API
  slug: dlocal-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-kyc-api-openapi.yml
- filename: dlocal-payment-methods-api-openapi.yml
  format: yaml
  label: dLocal Payment Methods API
  slug: dlocal-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payment-methods-api-openapi.yml
- filename: dlocal-payments-api-openapi.yml
  format: yaml
  label: dLocal Payments API
  slug: dlocal-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payments-api-openapi.yml
- filename: dlocal-payouts-api-openapi.yml
  format: yaml
  label: dLocal Payouts API
  slug: dlocal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payouts-api-openapi.yml
- filename: dlocal-refunds-api-openapi.yml
  format: yaml
  label: dLocal Refunds API
  slug: dlocal-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-refunds-api-openapi.yml
- filename: dlocal-tokens-api-openapi.yml
  format: yaml
  label: dLocal Tokens API
  slug: dlocal-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-tokens-api-openapi.yml
- filename: dlocal-transfers-api-openapi.yml
  format: yaml
  label: dLocal Transfers API
  slug: dlocal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-transfers-api-openapi.yml
- filename: dlocal-verifications-api-openapi.yml
  format: yaml
  label: dLocal Verifications API
  slug: dlocal-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-verifications-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dlocal Authentication
name_suffix: Authentication
oauth_flows: []
overview: dLocal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dLocal
provider_slug: dlocal
scheme_count: 1
schemes:
- description: 'HMAC-SHA256 signature. Format: "V2-HMAC-SHA256, Signature: {hmac_value}" Signature = HMAC-SHA256(X-Login + X-Date + RequestBody, SecretKey)'
  in: header
  name: HmacAuth
  parameter: Authorization
  sources:
  - openapi/dlocal-payins-openapi.yml
  - openapi/dlocal-payouts-openapi.yml
  - openapi/dlocal-platforms-openapi.yml
  - openapi/dlocal-verification-openapi.yml
  type: apiKey
slug: dlocal-authentication
source_filename: dlocal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dlocal-payins-openapi.yml, openapi/dlocal-payouts-openapi.yml, openapi/dlocal-platforms-openapi.yml,\n  openapi/dlocal-verification-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HmacAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'HMAC-SHA256 signature. Format: \"V2-HMAC-SHA256, Signature: {hmac_value}\" Signature\n    = HMAC-SHA256(X-Login + X-Date + RequestBody, SecretKey)'\n  sources:\n  - openapi/dlocal-payins-openapi.yml\n  - openapi/dlocal-payouts-openapi.yml\n  - openapi/dlocal-platforms-openapi.yml\n  - openapi/dlocal-verification-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/authentication/dlocal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Emerging Markets
- Payins
- Payouts
- Fintech
- Latin America
- Africa
- Asia
- Local Payment Methods
- Payment Processing
---
