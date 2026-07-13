---
api_key_in:
- header
api_specs:
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-hq-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Chart of Accounts & Company Objects API
  slug: campfire-hq-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-hq-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-hq-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-hq-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-hq-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-hq-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-hq-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-hq-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Integrations & Webhooks API
  slug: campfire-hq-integrations-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Campfire Hq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Campfire secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Campfire
provider_slug: campfire-hq
scheme_count: 1
schemes:
- description: 'Token-based (Knox) authentication. Send the header as: Authorization: Token <your-api-token>.'
  in: header
  name: knoxApiToken
  parameter: Authorization
  sources:
  - openapi/campfire-hq-openapi.yml
  type: apiKey
slug: campfire-hq-authentication
source_filename: campfire-hq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/campfire-hq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: knoxApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based (Knox) authentication. Send the header as: Authorization: Token\n    <your-api-token>.'\n  sources:\n  - openapi/campfire-hq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/authentication/campfire-hq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Accounting
- ERP
- General Ledger
- Revenue Recognition
- FinTech
- AI
---
