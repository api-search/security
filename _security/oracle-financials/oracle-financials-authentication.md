---
api_key_in: []
api_specs:
- filename: openapi-general-ledger.yaml
  format: yaml
  label: Oracle Financials General Ledger API
  slug: oracle-financials-general-ledger-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-general-ledger.yaml
- filename: openapi-payables.yaml
  format: yaml
  label: Oracle Financials Accounts Payable API
  slug: oracle-financials-accounts-payable-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-payables.yaml
- filename: openapi-receivables.yaml
  format: yaml
  label: Oracle Financials Accounts Receivable API
  slug: oracle-financials-accounts-receivable-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-receivables.yaml
- filename: openapi-cash-management.yaml
  format: yaml
  label: Oracle Financials Cash Management API
  slug: oracle-financials-cash-management-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-cash-management.yaml
- filename: openapi-expenses.yaml
  format: yaml
  label: Oracle Financials Expense Management API
  slug: oracle-financials-expense-management-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-expenses.yaml
- filename: openapi-fixed-assets.yaml
  format: yaml
  label: Oracle Financials Fixed Assets API
  slug: oracle-financials-fixed-assets-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-fixed-assets.yaml
- filename: openapi-reporting.yaml
  format: yaml
  label: Oracle Financial Reporting API
  slug: oracle-financial-reporting-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-reporting.yaml
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
