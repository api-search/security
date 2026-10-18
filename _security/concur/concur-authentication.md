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
- filename: concur-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Allocations API
  slug: concur-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-allocations-api-openapi.yml
- filename: concur-comments-api-openapi.yml
  format: yaml
  label: SAP Concur Comments API
  slug: concur-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-comments-api-openapi.yml
- filename: concur-expense-entries-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Entries API
  slug: concur-expense-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expense-entries-api-openapi.yml
- filename: concur-group-configurations-api-openapi.yml
  format: yaml
  label: SAP Concur Group Configurations API
  slug: concur-group-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-group-configurations-api-openapi.yml
- filename: concur-payment-batches-api-openapi.yml
  format: yaml
  label: SAP Concur Payment Batches API
  slug: concur-payment-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-payment-batches-api-openapi.yml
- filename: concur-quick-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Quick Expenses API
  slug: concur-quick-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-quick-expenses-api-openapi.yml
- filename: concur-receipt-images-api-openapi.yml
  format: yaml
  label: SAP Concur Receipt Images API
  slug: concur-receipt-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-receipt-images-api-openapi.yml
- filename: concur-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Reports API
  slug: concur-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-reports-api-openapi.yml
- filename: concur-workflows-api-openapi.yml
  format: yaml
  label: SAP Concur Workflows API
  slug: concur-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-workflows-api-openapi.yml
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
