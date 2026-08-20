---
api_key_in: []
api_specs:
- filename: target-inventory-api-openapi.yml
  format: yaml
  label: target Inventory API
  slug: target-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-inventory-api-openapi.yml
- filename: target-orders-api-openapi.yml
  format: yaml
  label: target Orders API
  slug: target-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-orders-api-openapi.yml
- filename: target-products-api-openapi.yml
  format: yaml
  label: target Products API
  slug: target-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-products-api-openapi.yml
- filename: target-search-api-openapi.yml
  format: yaml
  label: target Search API
  slug: target-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-search-api-openapi.yml
- filename: target-status-api-openapi.yml
  format: yaml
  label: target Status API
  slug: target-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-status-api-openapi.yml
- filename: target-stores-api-openapi.yml
  format: yaml
  label: target Stores API
  slug: target-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-stores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Target Authentication
name_suffix: Authentication
oauth_flows: []
overview: target secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: target
provider_slug: target
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/target-target-api-openapi.yml
  type: http
slug: target-authentication
source_filename: target-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/target-target-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/target-target-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/authentication/target-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 100
- E-Commerce
- Retail
- Product
- Inventory
- Stores
- Order
---
