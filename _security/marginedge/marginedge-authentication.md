---
api_key_in:
- header
api_specs:
- filename: marginedge-categories-api-openapi.yml
  format: yaml
  label: MarginEdge Categories API
  slug: marginedge-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/openapi/marginedge-categories-api-openapi.yml
- filename: marginedge-orders-api-openapi.yml
  format: yaml
  label: MarginEdge Orders API
  slug: marginedge-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/openapi/marginedge-orders-api-openapi.yml
- filename: marginedge-products-api-openapi.yml
  format: yaml
  label: MarginEdge Products API
  slug: marginedge-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/openapi/marginedge-products-api-openapi.yml
- filename: marginedge-restaurant-units-api-openapi.yml
  format: yaml
  label: MarginEdge Restaurant Units API
  slug: marginedge-restaurant-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/openapi/marginedge-restaurant-units-api-openapi.yml
- filename: marginedge-vendors-api-openapi.yml
  format: yaml
  label: MarginEdge Vendors API
  slug: marginedge-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/openapi/marginedge-vendors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Marginedge Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarginEdge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarginEdge
provider_slug: marginedge
scheme_count: 1
schemes:
- description: API key issued through the MarginEdge developer portal.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/marginedge-openapi.yml
  type: apiKey
slug: marginedge-authentication
source_filename: marginedge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marginedge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued through the MarginEdge developer portal.\n  sources:\n  - openapi/marginedge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/authentication/marginedge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Back Office
- Invoices
- Inventory
- Accounting
- Reporting
---
