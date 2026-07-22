---
api_key_in:
- header
api_specs:
- filename: nory-middleware-openapi.json
  format: json
  label: Nory Middleware API
  slug: nory-middleware
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-middleware-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nory secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nory
provider_slug: nory
scheme_count: 1
schemes:
- in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/nory-middleware-openapi.json
  type: apiKey
slug: nory-authentication
source_filename: nory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nory-middleware-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/nory-middleware-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/authentication/nory-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Restaurant
- Hospitality
- Inventory
- Workforce
- Payroll
- Point of Sale
- Artificial Intelligence
- Food and Beverage
---
