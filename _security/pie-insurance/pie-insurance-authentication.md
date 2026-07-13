---
api_key_in: []
api_specs:
- filename: pie-insurance-partner-api-openapi.yml
  format: yaml
  label: Pie Insurance Partner API
  slug: pie-insurance-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pie-insurance/refs/heads/main/openapi/pie-insurance-partner-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pie Insurance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pie Insurance secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pie Insurance
provider_slug: pie-insurance
scheme_count: 1
schemes:
- description: JWT Authorization header using the Bearer scheme. Enter token
  name: bearer
  scheme: Bearer
  sources:
  - openapi/pie-insurance-partner-api-openapi.yml
  type: http
slug: pie-insurance-authentication
source_filename: pie-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pie-insurance-partner-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: Bearer\n  description: JWT Authorization header using the Bearer scheme. Enter token\n  sources:\n  - openapi/pie-insurance-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pie-insurance/refs/heads/main/authentication/pie-insurance-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Insurtech
- Workers Compensation
- Small Business
- Commercial Insurance
- Business Owners Policy
- Commercial Auto
- General Liability
- Professional Liability
- Agency Portal
- Partner API
- Quoting
- Binding
---
