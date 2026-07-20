---
api_key_in:
- header
api_specs:
- filename: contalink-openapi-original.json
  format: json
  label: Contalink API
  slug: contalink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Contalink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contalink secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contalink
provider_slug: contalink
scheme_count: 1
schemes:
- description: Llave de API relacionada al usuario que hace la petición.
  in: header
  name: APIKey
  parameter: Authorization
  sources:
  - openapi/contalink-openapi-original.json
  type: apiKey
slug: contalink-authentication
source_filename: contalink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/contalink-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Llave de API relacionada al usuario que hace la petición.\n  sources:\n  - openapi/contalink-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/authentication/contalink-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Accounting
- Bookkeeping
- Payroll
- Tax
- Fintech
- Invoicing
- CFDI
- Mexico
- SaaS
---
