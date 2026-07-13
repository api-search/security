---
api_key_in: []
api_specs:
- filename: lowes-product-api-openapi.yml
  format: yaml
  label: Lowe's Product API
  slug: product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lowes/refs/heads/main/openapi/lowes-product-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lowes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lowe's secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lowe's
provider_slug: lowes
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lowes-product-api-openapi.yml
  type: http
slug: lowes-authentication
source_filename: lowes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lowes-product-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lowes-product-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lowes/refs/heads/main/authentication/lowes-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Home Improvement
- Products
- Retail
- Fortune 100
---
