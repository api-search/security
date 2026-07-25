---
api_key_in: []
api_specs:
- filename: oracle-financials-budgetary-control-api-openapi.yml
  format: yaml
  label: Oracle Financials Budgetary Control API
  slug: oracle-financials-budgetary-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-budgetary-control-api-openapi.yml
- filename: oracle-financials-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Oracle Financials Chart of Accounts API
  slug: oracle-financials-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-chart-of-accounts-api-openapi.yml
- filename: oracle-financials-currency-rates-api-openapi.yml
  format: yaml
  label: Oracle Financials Currency Rates API
  slug: oracle-financials-currency-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-currency-rates-api-openapi.yml
- filename: oracle-financials-journal-batches-api-openapi.yml
  format: yaml
  label: Oracle Financials Journal Batches API
  slug: oracle-financials-journal-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-journal-batches-api-openapi.yml
- filename: oracle-financials-ledger-balances-api-openapi.yml
  format: yaml
  label: Oracle Financials Ledger Balances API
  slug: oracle-financials-ledger-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-ledger-balances-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Financials Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Financials secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle Financials
provider_slug: oracle-financials
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from Oracle Identity Cloud Service
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-financials-general-ledger-openapi.yml
  type: http
slug: oracle-financials-authentication
source_filename: oracle-financials-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-financials-general-ledger-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from Oracle Identity Cloud Service\n  sources:\n  - openapi/oracle-financials-general-ledger-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/authentication/oracle-financials-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Accounts Payable
- Accounts Receivable
- Cash Management
- ERP
- Expense Management
- Financial Management
- General Ledger
---
