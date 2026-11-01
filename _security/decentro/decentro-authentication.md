---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: decentro-kyc-api-openapi.yml
  format: yaml
  label: Decentro KYC & Onboarding API
  slug: kyc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-kyc-api-openapi.yml
- filename: decentro-virtual-accounts-api-openapi.yml
  format: yaml
  label: Decentro Virtual Accounts API
  slug: virtual-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-virtual-accounts-api-openapi.yml
- filename: decentro-accounts-api-openapi.yml
  format: yaml
  label: Decentro Accounts API
  slug: decentro-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-accounts-api-openapi.yml
- filename: decentro-forensics-api-openapi.yml
  format: yaml
  label: Decentro Forensics API
  slug: decentro-forensics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-forensics-api-openapi.yml
- filename: decentro-journals-api-openapi.yml
  format: yaml
  label: Decentro Journals API
  slug: decentro-journals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-journals-api-openapi.yml
- filename: decentro-transactions-api-openapi.yml
  format: yaml
  label: Decentro Transactions API
  slug: decentro-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-transactions-api-openapi.yml
- filename: decentro-verification-api-openapi.yml
  format: yaml
  label: Decentro Verification API
  slug: decentro-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-verification-api-openapi.yml
- filename: decentro-auth-api-openapi.yml
  format: yaml
  label: Decentro Auth API
  slug: decentro-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-auth-api-openapi.yml
- filename: decentro-banking-api-openapi.yml
  format: yaml
  label: Decentro Banking API
  slug: decentro-banking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-banking-api-openapi.yml
- filename: decentro-decentro-api-openapi.yml
  format: yaml
  label: Decentro Decentro API
  slug: decentro-decentro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-decentro-api-openapi.yml
- filename: decentro-deposit-simulation-api-openapi.yml
  format: yaml
  label: Decentro Deposit Simulation API
  slug: decentro-deposit-simulation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-deposit-simulation-api-openapi.yml
- filename: decentro-payments-api-openapi.yml
  format: yaml
  label: Decentro Payments API
  slug: decentro-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decentro/openapi/decentro-payments-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/decentro/authentication/decentro-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Banking
- Banking as a Service
- Fintech
- India
- KYC
- Ledger
- Payments
- UPI
- Virtual Accounts
---
