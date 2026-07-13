---
api_key_in: []
api_specs:
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Orders API
  slug: extensiv-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Inventory API
  slug: extensiv-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Items API
  slug: extensiv-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Customers API
  slug: extensiv-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Receivers (ASN) API
  slug: extensiv-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Warehouses API
  slug: extensiv-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Auth Token API
  slug: extensiv-auth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Extensiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Extensiv secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Extensiv
provider_slug: extensiv
scheme_count: 2
schemes:
- description: Base64-encoded "Client ID:Client Secret" used only against /AuthServer/api/Token.
  name: basicClientCredentials
  scheme: basic
  sources:
  - openapi/extensiv-openapi.yml
  type: http
- bearerFormat: JWT
  description: Short-lived bearer access token minted by the auth server.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/extensiv-openapi.yml
  type: http
slug: extensiv-authentication
source_filename: extensiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/extensiv-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicClientCredentials\n  type: http\n  scheme: basic\n  description: Base64-encoded \"Client ID:Client Secret\" used only against /AuthServer/api/Token.\n  sources:\n  - openapi/extensiv-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived bearer access token minted by the auth server.\n  sources:\n  - openapi/extensiv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/authentication/extensiv-authentication.yml
summary_line: http · 2 schemes
tags:
- 3PL
- Warehouse Management
- WMS
- Order Management
- Inventory Management
- Fulfillment
- Logistics
- Supply Chain
---
