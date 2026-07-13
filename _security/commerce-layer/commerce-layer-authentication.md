---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Commerce Layer Core API
  slug: commerce-layer-core-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/openapi.json
- filename: openapi.json
  format: json
  label: Commerce Layer Provisioning API
  slug: commerce-layer-provisioning-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/provisioning/openapi.json
- filename: openapi.json
  format: json
  label: Commerce Layer Metrics API
  slug: commerce-layer-metrics-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/metrics/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Commerce Layer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commerce Layer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Commerce Layer
provider_slug: commerce-layer
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commerce-layer-core-api-openapi.json
  - openapi/commerce-layer-metrics-api-openapi.json
  - openapi/commerce-layer-provisioning-api-openapi.json
  type: http
slug: commerce-layer-authentication
source_filename: commerce-layer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/commerce-layer-core-api-openapi.json, openapi/commerce-layer-metrics-api-openapi.json,\n  openapi/commerce-layer-provisioning-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/commerce-layer-core-api-openapi.json\n  - openapi/commerce-layer-metrics-api-openapi.json\n  - openapi/commerce-layer-provisioning-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerce-layer/refs/heads/main/authentication/commerce-layer-authentication.yml
summary_line: http · 1 scheme
tags:
- Headless Commerce
- Composable Commerce
- API-First
- Ecommerce
- JSON:API
- OAuth 2.0
- Multi-Market
- Multi-Currency
- B2C
- B2B
- Subscriptions
- Promotions
- Inventory
- Order Management
- Checkout
---
