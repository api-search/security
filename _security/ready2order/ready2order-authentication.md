---
api_key_in:
- header
api_specs:
- filename: ready2order-openapi-original.json
  format: json
  label: ready2order Public API
  slug: ready2order-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready2order/refs/heads/main/openapi/ready2order-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ready2Order Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ready2order secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ready2order
provider_slug: ready2order
scheme_count: 1
schemes:
- description: Account Token obtained after completing the authorization flow. See First Steps for details.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/ready2order-openapi-original.json
  type: apiKey
slug: ready2order-authentication
source_filename: ready2order-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/ready2order-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Account Token obtained after completing the authorization flow. See First Steps\n    for details.\n  sources:\n  - openapi/ready2order-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ready2order/refs/heads/main/authentication/ready2order-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Point of Sale
- POS
- Payments
- Retail
- Gastronomy
- Cash Register
- SaaS
---
