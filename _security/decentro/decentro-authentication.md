---
api_key_in:
- header
api_specs:
- filename: decentro-kyc-api-openapi.yml
  format: yaml
  label: Decentro KYC & Onboarding API
  slug: kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-kyc-api-openapi.yml
- filename: decentro-payments-api-openapi.yml
  format: yaml
  label: Decentro Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-payments-api-openapi.yml
- filename: decentro-virtual-accounts-api-openapi.yml
  format: yaml
  label: Decentro Virtual Accounts API
  slug: virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-virtual-accounts-api-openapi.yml
- filename: decentro-ledger-api-openapi.yml
  format: yaml
  label: Decentro Ledger API
  slug: ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/openapi/decentro-ledger-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Decentro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Decentro secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Decentro
provider_slug: decentro
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: client_secret
  sources:
  - openapi/decentro-kyc-api-openapi.yml
  - openapi/decentro-ledger-api-openapi.yml
  - openapi/decentro-payments-api-openapi.yml
  - openapi/decentro-virtual-accounts-api-openapi.yml
  type: apiKey
slug: decentro-authentication
source_filename: decentro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/decentro-kyc-api-openapi.yml, openapi/decentro-ledger-api-openapi.yml, openapi/decentro-payments-api-openapi.yml,\n  openapi/decentro-virtual-accounts-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: client_secret\n  sources:\n  - openapi/decentro-kyc-api-openapi.yml\n  - openapi/decentro-ledger-api-openapi.yml\n  - openapi/decentro-payments-api-openapi.yml\n  - openapi/decentro-virtual-accounts-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/authentication/decentro-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Banking
- Banking-as-a-Service
- FinTech
- India
- KYC
- Ledger
- Payments
- UPI
- Virtual Accounts
---
