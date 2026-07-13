---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Payfit Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayFit secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PayFit
provider_slug: payfit
scheme_count: 2
schemes:
- description: OAuth 2.0 bearer token for Partner API integrations.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/payfit-openapi.yml
  type: http
- description: Private API key for Customer API direct access.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/payfit-openapi.yml
  type: apiKey
slug: payfit-authentication
source_filename: payfit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/payfit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token for Partner API integrations.\n  sources:\n  - openapi/payfit-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Private API key for Customer API direct access.\n  sources:\n  - openapi/payfit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payfit/refs/heads/main/authentication/payfit-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payroll
- Human Resources
- HR Tech
- Europe Payroll
- Time and Attendance
- Employee Management
---
