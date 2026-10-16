---
anonymous_access: false
api_key_in: []
api_specs:
- filename: concur-expense-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Reports API
  slug: concur-expense-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expense-reports-api-openapi.yml
- filename: concur-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expenses API
  slug: concur-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expenses-api-openapi.yml
- filename: sap-concur-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Allocations API
  slug: sap-concur-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-allocations-api-openapi.yml
- filename: sap-concur-comments-api-openapi.yml
  format: yaml
  label: SAP Concur Comments API
  slug: sap-concur-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-comments-api-openapi.yml
- filename: sap-concur-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expenses API
  slug: sap-concur-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expenses-api-openapi.yml
- filename: sap-concur-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Reports API
  slug: sap-concur-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-reports-api-openapi.yml
- filename: sap-concur-workflows-api-openapi.yml
  format: yaml
  label: SAP Concur Workflows API
  slug: sap-concur-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-workflows-api-openapi.yml
- filename: sap-concur-expense-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Allocations API
  slug: sap-concur-expense-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-allocations-api-openapi.yml
- filename: sap-concur-expense-expense-entries-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Entries API
  slug: sap-concur-expense-expense-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-expense-entries-api-openapi.yml
- filename: sap-concur-expense-expense-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Reports API
  slug: sap-concur-expense-expense-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-expense-reports-api-openapi.yml
- filename: sap-concur-expense-group-configurations-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Group Configurations API
  slug: sap-concur-expense-group-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-group-configurations-api-openapi.yml
- filename: sap-concur-expense-payment-batches-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Payment Batches API
  slug: sap-concur-expense-payment-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-payment-batches-api-openapi.yml
- filename: sap-concur-expense-quick-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Quick Expenses API
  slug: sap-concur-expense-quick-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-quick-expenses-api-openapi.yml
- filename: sap-concur-expense-receipt-images-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Receipt Images API
  slug: sap-concur-expense-receipt-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-receipt-images-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Concur Authentication
name_suffix: Authentication
oauth_flows: []
overview: SAP Concur secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SAP Concur
provider_slug: concur
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer Token authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/concur-expense-api.yaml
  type: http
slug: concur-authentication
source_filename: concur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/concur-expense-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer Token authentication.\n  sources:\n  - openapi/concur-expense-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/authentication/concur-authentication.yml
summary_line: http · 1 scheme
tags:
- Expense Management
- Finance
- Invoices
- SAP
- Travel
- Business Travel
- Financial Services
- Invoice Management
- Travel Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
---
