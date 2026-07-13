---
api_key_in: []
api_specs:
- filename: printify-openapi.yml
  format: yaml
  label: Printify Shops API
  slug: printify-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Catalog API
  slug: printify-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Products API
  slug: printify-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Orders API
  slug: printify-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Uploads API
  slug: printify-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Webhooks API
  slug: printify-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Printify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Printify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Printify
provider_slug: printify
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Personal Access Token or OAuth 2.0 access token sent as Authorization: Bearer {token}. A User-Agent header is also required.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/printify-openapi.yml
  type: http
slug: printify-authentication
source_filename: printify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/printify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Personal Access Token or OAuth 2.0 access token sent as Authorization: Bearer\n    {token}. A User-Agent header is also required.'\n  sources:\n  - openapi/printify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/authentication/printify-authentication.yml
summary_line: http · 1 scheme
tags:
- Print on Demand
- Ecommerce
- Marketplace
- Fulfillment
- Merchandise
---
