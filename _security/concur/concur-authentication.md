---
api_key_in: []
api_specs:
- filename: concur-expense-api.yaml
  format: yaml
  label: SAP Concur Expense API
  slug: expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expense-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
- Invoice
- SAP
- Travel
---
