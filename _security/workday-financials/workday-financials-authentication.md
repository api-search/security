---
api_key_in: []
api_specs:
- filename: Financial_Management.json
  format: json
  label: Workday Financial Management API
  slug: workday-financial-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Financial_Management/v38.2/Financial_Management.json
- filename: Revenue_Management.json
  format: json
  label: Workday Revenue Management API
  slug: workday-revenue-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Revenue_Management/v38.2/Revenue_Management.json
- filename: Expenses.json
  format: json
  label: Workday Expenses API
  slug: workday-expenses-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Expenses/v38.2/Expenses.json
- filename: Resource_Management.json
  format: json
  label: Workday Procurement API
  slug: workday-procurement-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Resource_Management/v38.2/Resource_Management.json
- filename: Cash_Management.json
  format: json
  label: Workday Cash Management API
  slug: workday-cash-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Cash_Management/v38.2/Cash_Management.json
- filename: Financial_Management.json
  format: json
  label: Workday Financial Accounting API
  slug: workday-financial-accounting-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Financial_Management/v38.2/Financial_Management.json
- filename: Report_as_a_Service.json
  format: json
  label: Workday Reporting API
  slug: workday-reporting-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Report_as_a_Service/v38.2/Report_as_a_Service.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workday Financials Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workday Financials secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workday Financials
provider_slug: workday-financials
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from Workday authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workday-financials-cash-management-openapi.yml
  - openapi/workday-financials-expenses-openapi.yml
  - openapi/workday-financials-financial-accounting-openapi.yml
  - openapi/workday-financials-financial-management-openapi.yml
  - openapi/workday-financials-procurement-openapi.yml
  - openapi/workday-financials-reporting-openapi.yml
  - openapi/workday-financials-revenue-management-openapi.yml
  type: http
slug: workday-financials-authentication
source_filename: workday-financials-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-financials-cash-management-openapi.yml, openapi/workday-financials-expenses-openapi.yml,\n  openapi/workday-financials-financial-accounting-openapi.yml, openapi/workday-financials-financial-management-openapi.yml,\n  openapi/workday-financials-procurement-openapi.yml, openapi/workday-financials-reporting-openapi.yml,\n  openapi/workday-financials-revenue-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from Workday authentication\n  sources:\n  - openapi/workday-financials-cash-management-openapi.yml\n  - openapi/workday-financials-expenses-openapi.yml\n  - openapi/workday-financials-financial-accounting-openapi.yml\n  - openapi/workday-financials-financial-management-openapi.yml\n  - openapi/workday-financials-procurement-openapi.yml\n  - openapi/workday-financials-reporting-openapi.yml\n\
  \  - openapi/workday-financials-revenue-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-financials/refs/heads/main/authentication/workday-financials-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Cloud ERP
- Financial Management
- Procurement
---
