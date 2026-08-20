---
api_key_in:
- header
api_specs:
- filename: campfire-hq-accounts-payable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-hq-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-accounts-payable-api-openapi.yml
- filename: campfire-hq-accounts-receivable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-hq-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-accounts-receivable-api-openapi.yml
- filename: campfire-hq-bank-reconciliation-api-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-hq-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-bank-reconciliation-api-openapi.yml
- filename: campfire-hq-cash-management-api-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-hq-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-cash-management-api-openapi.yml
- filename: campfire-hq-coa-api-openapi.yml
  format: yaml
  label: Campfire coa API
  slug: campfire-hq-coa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-coa-api-openapi.yml
- filename: campfire-hq-company-objects-api-openapi.yml
  format: yaml
  label: Campfire Company Objects API
  slug: campfire-hq-company-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-company-objects-api-openapi.yml
- filename: campfire-hq-core-accounting-api-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-hq-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-core-accounting-api-openapi.yml
- filename: campfire-hq-custom-fields-api-openapi.yml
  format: yaml
  label: Campfire Custom Fields API
  slug: campfire-hq-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-custom-fields-api-openapi.yml
- filename: campfire-hq-financial-statements-api-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-hq-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-financial-statements-api-openapi.yml
- filename: campfire-hq-integrations-api-openapi.yml
  format: yaml
  label: Campfire Integrations API
  slug: campfire-hq-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-integrations-api-openapi.yml
- filename: campfire-hq-revenue-recognition-api-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-hq-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-revenue-recognition-api-openapi.yml
- filename: campfire-hq-settings-api-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-hq-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-settings-api-openapi.yml
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
- Fintech
- Artificial Intelligence
---
