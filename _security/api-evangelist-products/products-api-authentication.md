---
api_key_in:
- header
api_specs:
- filename: products-api-openapi.yml
  format: yaml
  label: Products API.
  slug: products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-products/refs/heads/main/openapi/products-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Products Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Products secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Products
provider_slug: api-evangelist-products
scheme_count: 1
schemes:
- in: header
  name: apiKeys
  parameter: api-key
  sources:
  - openapi/products-api-openapi.yml
  type: apiKey
slug: products-api-authentication
source_filename: products-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/products-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeys\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/products-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-products/refs/heads/main/authentication/products-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Programming Interface
- Products
---
