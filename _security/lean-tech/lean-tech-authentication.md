---
api_key_in: []
api_specs:
- filename: lean-authentication-api-openapi.yml
  format: yaml
  label: Lean Authentication API
  slug: lean-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-authentication-api-openapi.yml
- filename: lean-customers-api-openapi.yml
  format: yaml
  label: Lean Customers API
  slug: lean-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-customers-api-openapi.yml
- filename: lean-entities-api-openapi.yml
  format: yaml
  label: Lean Entities API
  slug: lean-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-entities-api-openapi.yml
- filename: lean-data-api-openapi.yml
  format: yaml
  label: Lean Data API
  slug: lean-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-data-api-openapi.yml
- filename: lean-insights-api-openapi.yml
  format: yaml
  label: Lean Insights API
  slug: lean-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-insights-api-openapi.yml
- filename: lean-banks-api-openapi.yml
  format: yaml
  label: Lean Banks API
  slug: lean-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-banks-api-openapi.yml
- filename: lean-verifications-api-openapi.yml
  format: yaml
  label: Lean Verifications API
  slug: lean-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-verifications-api-openapi.yml
- filename: lean-payments-api-openapi.yml
  format: yaml
  label: Lean Payments API
  slug: lean-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payments-api-openapi.yml
- filename: lean-payment-sources-api-openapi.yml
  format: yaml
  label: Lean Payment Sources API
  slug: lean-payment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payment-sources-api-openapi.yml
- filename: lean-payouts-api-openapi.yml
  format: yaml
  label: Lean Payouts API
  slug: lean-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payouts-api-openapi.yml
- filename: lean-refunds-api-openapi.yml
  format: yaml
  label: Lean Refunds API
  slug: lean-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-refunds-api-openapi.yml
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
