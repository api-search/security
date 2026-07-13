---
api_key_in: []
api_specs:
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Applications API
  slug: unit-co-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Customers API
  slug: unit-co-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Accounts API
  slug: unit-co-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Cards API
  slug: unit-co-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Card Authorizations API
  slug: unit-co-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Payments API
  slug: unit-co-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Counterparties API
  slug: unit-co-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Checks API
  slug: unit-co-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Transactions API
  slug: unit-co-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Statements and Tax Forms API
  slug: unit-co-statements-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Events and Webhooks API
  slug: unit-co-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Risk and Fraud Prevention API
  slug: unit-co-risk-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Credit and Repayments API
  slug: unit-co-credit-repayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Fees and Rewards API
  slug: unit-co-fees-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit API Tokens API
  slug: unit-co-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unit Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unit
provider_slug: unit-co
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer JWT issued as an org API token (Dashboard > Developers) or a customer API token. Sent as `Authorization: Bearer ${TOKEN}`. All request and response bodies use the `application/vnd.api+json` JSON:API media type.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/unit-co-openapi.yml
  type: http
slug: unit-co-authentication
source_filename: unit-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unit-co-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Bearer JWT issued as an org API token (Dashboard > Developers) or a customer\n    API token. Sent as `Authorization: Bearer ${TOKEN}`. All request and response bodies use\n    the `application/vnd.api+json` JSON:API media type.'\n  sources:\n  - openapi/unit-co-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/authentication/unit-co-authentication.yml
summary_line: http · 1 scheme
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
- Lending
- JSON:API
---
