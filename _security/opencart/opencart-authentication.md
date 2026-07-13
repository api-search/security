---
api_key_in:
- query
api_specs:
- filename: opencart-rest-api.yml
  format: yaml
  label: OpenCart REST API
  slug: opencart-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencart/refs/heads/main/openapi/opencart-rest-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opencart Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenCart secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenCart
provider_slug: opencart
scheme_count: 1
schemes:
- description: Session token obtained from the /login endpoint
  in: query
  name: apiToken
  parameter: api_token
  sources:
  - openapi/opencart-rest-api.yml
  type: apiKey
slug: opencart-authentication
source_filename: opencart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opencart-rest-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: Session token obtained from the /login endpoint\n  sources:\n  - openapi/opencart-rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencart/refs/heads/main/authentication/opencart-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- eCommerce
- Shopping Cart
- Open Source
- Self-Hosted
- Products
- Orders
- Customers
- Categories
---
