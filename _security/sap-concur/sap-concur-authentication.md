---
api_key_in: []
api_specs:
- filename: expense-report.json
  format: json
  label: Concur Expense API
  slug: concur-expense-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/expense/expense-report/expense-report.json
- filename: itinerary.json
  format: json
  label: Concur Travel API
  slug: concur-travel-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/travel/itinerary/itinerary.json
- filename: v3.invoice.json
  format: json
  label: Concur Invoice API
  slug: concur-invoice-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/invoice/v3.invoice.json
- filename: v4.request.json
  format: json
  label: Concur Request API
  slug: concur-request-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/request/v4.request.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sap Concur Authentication
name_suffix: Authentication
oauth_flows: []
overview: SAP Concur secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SAP Concur
provider_slug: sap-concur
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token. Obtain tokens via the SAP Concur Authentication API using either Company or User level grants. Required scopes vary by operation.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sap-concur-expense-openapi.yml
  type: http
slug: sap-concur-authentication
source_filename: sap-concur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-concur-expense-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token. Obtain tokens via the SAP Concur Authentication API using\n    either Company or User level grants. Required scopes vary by operation.\n  sources:\n  - openapi/sap-concur-expense-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/authentication/sap-concur-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
---
