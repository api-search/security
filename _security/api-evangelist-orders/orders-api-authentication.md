---
api_key_in:
- header
api_specs:
- filename: orders-api-openapi.yml
  format: yaml
  label: Orders API.
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-orders/refs/heads/main/openapi/orders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Orders Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orders secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orders
provider_slug: api-evangelist-orders
scheme_count: 1
schemes:
- in: header
  name: apiKeys
  parameter: api-key
  sources:
  - openapi/orders-api-openapi.yml
  type: apiKey
slug: orders-api-authentication
source_filename: orders-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orders-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeys\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/orders-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-orders/refs/heads/main/authentication/orders-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Programming Interface
- Orders
---
