---
api_key_in:
- header
api_specs:
- filename: mono-co-account-information-api-openapi.yml
  format: yaml
  label: Mono Account Information API
  slug: mono-co-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-account-information-api-openapi.yml
- filename: mono-co-account-linking-api-openapi.yml
  format: yaml
  label: Mono Account Linking API
  slug: mono-co-account-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-account-linking-api-openapi.yml
- filename: mono-co-direct-debit-api-openapi.yml
  format: yaml
  label: Mono Direct Debit API
  slug: mono-co-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-direct-debit-api-openapi.yml
- filename: mono-co-directpay-api-openapi.yml
  format: yaml
  label: Mono DirectPay API
  slug: mono-co-directpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-directpay-api-openapi.yml
- filename: mono-co-identity-and-income-api-openapi.yml
  format: yaml
  label: Mono Identity and Income API
  slug: mono-co-identity-and-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-identity-and-income-api-openapi.yml
- filename: mono-co-transactions-and-statements-api-openapi.yml
  format: yaml
  label: Mono Transactions and Statements API
  slug: mono-co-transactions-and-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-transactions-and-statements-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mono Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mono secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mono
provider_slug: mono-co
scheme_count: 1
schemes:
- description: Secret application key issued in the Mono dashboard.
  in: header
  name: monoSecKey
  parameter: mono-sec-key
  sources:
  - openapi/mono-co-openapi.yml
  type: apiKey
slug: mono-co-authentication
source_filename: mono-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mono-co-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: monoSecKey\n  type: apiKey\n  in: header\n  parameter: mono-sec-key\n  description: Secret application key issued in the Mono dashboard.\n  sources:\n  - openapi/mono-co-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/authentication/mono-co-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Banking
- Financial Data
- Payments
- Direct Debit
- Africa
---
