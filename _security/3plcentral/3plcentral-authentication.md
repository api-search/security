---
api_key_in: []
api_specs:
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Orders API
  slug: 3plcentral-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Items API
  slug: 3plcentral-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Inventory API
  slug: 3plcentral-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Stock Summaries API
  slug: 3plcentral-stock-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Receivers (ASN) API
  slug: 3plcentral-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Customers API
  slug: 3plcentral-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Warehouses API
  slug: 3plcentral-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Packages API
  slug: 3plcentral-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 3Plcentral Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3PL Warehouse Manager secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 3PL Warehouse Manager
provider_slug: 3plcentral
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Short-lived access token from POST /AuthServer/api/Token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/3plcentral-openapi.yml
  type: http
- description: Base64-encoded "clientId:clientSecret" used only to obtain a token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/3plcentral-openapi.yml
  type: http
slug: 3plcentral-authentication
source_filename: 3plcentral-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/3plcentral-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived access token from POST /AuthServer/api/Token.\n  sources:\n  - openapi/3plcentral-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Base64-encoded \"clientId:clientSecret\" used only to obtain a token.\n  sources:\n  - openapi/3plcentral-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/authentication/3plcentral-authentication.yml
summary_line: http · 2 schemes
tags:
- Warehouse Management
- WMS
- 3PL
- Logistics
- Fulfillment
- Inventory
- Orders
- SecureWMS
- Extensiv
---
