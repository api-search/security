---
api_key_in: []
api_specs:
- filename: sap-concur-expense-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Allocations API
  slug: sap-concur-expense-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-allocations-api-openapi.yml
- filename: sap-concur-expense-expense-entries-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Expense Entries API
  slug: sap-concur-expense-expense-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-expense-entries-api-openapi.yml
- filename: sap-concur-expense-expense-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Expense Reports API
  slug: sap-concur-expense-expense-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-expense-reports-api-openapi.yml
- filename: sap-concur-expense-group-configurations-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Group Configurations API
  slug: sap-concur-expense-group-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-group-configurations-api-openapi.yml
- filename: sap-concur-expense-payment-batches-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Payment Batches API
  slug: sap-concur-expense-payment-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-payment-batches-api-openapi.yml
- filename: sap-concur-expense-quick-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Quick Expenses API
  slug: sap-concur-expense-quick-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-quick-expenses-api-openapi.yml
- filename: sap-concur-expense-receipt-images-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Receipt Images API
  slug: sap-concur-expense-receipt-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-receipt-images-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Concur Expense Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SAP Concur Expense secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SAP Concur Expense
provider_slug: sap-concur-expense
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://us.api.concursolutions.com/oauth2/v0/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://us.api.concursolutions.com/oauth2/v0/token
  name: OAuth2
  sources:
  - openapi/sap-concur-expense-report-openapi.yml
  type: oauth2
slug: sap-concur-expense-authentication
source_filename: sap-concur-expense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-concur-expense-report-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us.api.concursolutions.com/oauth2/v0/authorize\n    tokenUrl: https://us.api.concursolutions.com/oauth2/v0/token\n    scopes: 3\n  sources:\n  - openapi/sap-concur-expense-report-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/authentication/sap-concur-expense-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Expense Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
- SAP
- Travel
---
