---
api_key_in:
- header
api_specs:
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Account Holders API
  slug: lithic-com-account-holders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Accounts API
  slug: lithic-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Cards API
  slug: lithic-com-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Transactions & Authorizations API
  slug: lithic-com-transactions-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Authorization Rules API
  slug: lithic-com-authorization-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Real-Time Decisioning API
  slug: lithic-com-realtime-decisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Disputes API
  slug: lithic-com-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Events & Webhooks API
  slug: lithic-com-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Financial Accounts & Statements API
  slug: lithic-com-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Balances & Holds API
  slug: lithic-com-balances-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Payments (ACH) API
  slug: lithic-com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Ledger, Transfers & Settlement API
  slug: lithic-com-ledger-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic External Payments & Bank Accounts API
  slug: lithic-com-external-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Tokenization & Digital Wallets API
  slug: lithic-com-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Fraud & Transaction Monitoring API
  slug: lithic-com-fraud-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lithic Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lithic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lithic
provider_slug: lithic-com
scheme_count: 1
schemes:
- description: Raw API secret key value (not prefixed with "Bearer").
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/lithic-com-openapi.yml
  type: apiKey
slug: lithic-com-authentication
source_filename: lithic-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lithic-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Raw API secret key value (not prefixed with \"Bearer\").\n  sources:\n  - openapi/lithic-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/authentication/lithic-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fintech
- Card Issuing
- Payments
- Issuer Processor
- KYC
- Banking as a Service
---
