---
api_key_in:
- header
api_specs:
- filename: mono-co-openapi.yml
  format: yaml
  label: Account Linking and Auth
  slug: account-linking-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Account Information
  slug: account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Transactions and Statements
  slug: transactions-statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Identity and Income
  slug: identity-income
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: DirectPay Payments
  slug: directpay-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Direct Debit and Mandates
  slug: direct-debit-mandates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
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
