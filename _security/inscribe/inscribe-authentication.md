---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: inscribe-bank-accounts-api-openapi.yml
  format: yaml
  label: Inscribe Bank Accounts API
  slug: inscribe-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-bank-accounts-api-openapi.yml
- filename: inscribe-collect-sessions-api-openapi.yml
  format: yaml
  label: Inscribe Collect Sessions API
  slug: inscribe-collect-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-collect-sessions-api-openapi.yml
- filename: inscribe-credit-insights-api-openapi.yml
  format: yaml
  label: Inscribe Credit Insights API
  slug: inscribe-credit-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-credit-insights-api-openapi.yml
- filename: inscribe-customers-api-openapi.yml
  format: yaml
  label: Inscribe Customers API
  slug: inscribe-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-customers-api-openapi.yml
- filename: inscribe-documents-api-openapi.yml
  format: yaml
  label: Inscribe Documents API
  slug: inscribe-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-documents-api-openapi.yml
- filename: inscribe-open-banking-api-openapi.yml
  format: yaml
  label: Inscribe Open Banking API
  slug: inscribe-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-open-banking-api-openapi.yml
- filename: inscribe-reachability-check-api-openapi.yml
  format: yaml
  label: Inscribe Reachability Check API
  slug: inscribe-reachability-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-reachability-check-api-openapi.yml
- filename: inscribe-transactions-api-openapi.yml
  format: yaml
  label: Inscribe Transactions API
  slug: inscribe-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Inscribe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inscribe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inscribe
provider_slug: inscribe
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/inscribe-core-resources-openapi.yml
  type: apiKey
slug: inscribe-authentication
source_filename: inscribe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/inscribe-core-resources-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/inscribe-core-resources-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/authentication/inscribe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fraud Prevention
- Document Verification
- Financial Services
- KYC
- KYB
- Bank Statements
- Paystubs
- Identity Verification
- Risk Management
- Fintech
- Artificial Intelligence
- Machine Learning
---
