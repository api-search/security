---
api_key_in:
- header
api_specs:
- filename: d-local-payments-api-openapi.yml
  format: yaml
  label: dLocal Payments API
  slug: d-local-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-payments-api-openapi.yml
- filename: d-local-refunds-api-openapi.yml
  format: yaml
  label: dLocal Refunds API
  slug: d-local-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-refunds-api-openapi.yml
- filename: d-local-cards-api-openapi.yml
  format: yaml
  label: dLocal Cards API
  slug: d-local-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-cards-api-openapi.yml
- filename: d-local-payouts-v3-api-openapi.yml
  format: yaml
  label: dLocal Payouts V3 API
  slug: d-local-payouts-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-payouts-v3-api-openapi.yml
- filename: d-local-platforms-api-openapi.yml
  format: yaml
  label: dLocal For Platforms API
  slug: d-local-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-platforms-api-openapi.yml
- filename: d-local-kyc-verifications-api-openapi.yml
  format: yaml
  label: dLocal KYC Verifications API
  slug: d-local-kyc-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-kyc-verifications-api-openapi.yml
- filename: d-local-chargebacks-api-openapi.yml
  format: yaml
  label: dLocal Chargebacks API
  slug: d-local-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-chargebacks-api-openapi.yml
- filename: d-local-enrollments-api-openapi.yml
  format: yaml
  label: dLocal Enrollments API
  slug: d-local-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-enrollments-api-openapi.yml
- filename: d-local-exchange-rates-api-openapi.yml
  format: yaml
  label: dLocal Exchange Rates API
  slug: d-local-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-exchange-rates-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: D Local Authentication
name_suffix: Authentication
oauth_flows: []
overview: dLocal secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: dLocal
provider_slug: d-local
scheme_count: 2
schemes:
- in: header
  name: dLocalSignature
  parameter: Authorization
  sources:
  - openapi/d-local-cards-api-openapi.yml
  - openapi/d-local-chargebacks-api-openapi.yml
  - openapi/d-local-enrollments-api-openapi.yml
  - openapi/d-local-exchange-rates-api-openapi.yml
  - openapi/d-local-kyc-verifications-api-openapi.yml
  - openapi/d-local-payments-api-openapi.yml
  - openapi/d-local-refunds-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/d-local-payouts-v3-api-openapi.yml
  - openapi/d-local-platforms-api-openapi.yml
  type: http
slug: d-local-authentication
source_filename: d-local-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/d-local-cards-api-openapi.yml, openapi/d-local-chargebacks-api-openapi.yml,\n  openapi/d-local-enrollments-api-openapi.yml, openapi/d-local-exchange-rates-api-openapi.yml,\n  openapi/d-local-kyc-verifications-api-openapi.yml, openapi/d-local-payments-api-openapi.yml,\n  openapi/d-local-payouts-v3-api-openapi.yml, openapi/d-local-platforms-api-openapi.yml, openapi/d-local-refunds-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: dLocalSignature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/d-local-cards-api-openapi.yml\n  - openapi/d-local-chargebacks-api-openapi.yml\n  - openapi/d-local-enrollments-api-openapi.yml\n  - openapi/d-local-exchange-rates-api-openapi.yml\n  - openapi/d-local-kyc-verifications-api-openapi.yml\n  - openapi/d-local-payments-api-openapi.yml\n  - openapi/d-local-refunds-api-openapi.yml\n- name: bearerAuth\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/d-local-payouts-v3-api-openapi.yml\n  - openapi/d-local-platforms-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/authentication/d-local-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- Payouts
- EmergingMarkets
- LatAm
- Africa
- Asia
- FX
- Fintech
---
