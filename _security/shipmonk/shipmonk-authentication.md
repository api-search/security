---
api_key_in:
- header
api_specs:
- filename: shipmonk-webhooks-asyncapi.yml
  format: yaml
  label: ShipMonk Webhooks
  slug: shipmonk-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/asyncapi/shipmonk-webhooks-asyncapi.yml
- filename: shipmonk-orders-api-openapi.yml
  format: yaml
  label: ShipMonk Orders API
  slug: shipmonk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-orders-api-openapi.yml
- filename: shipmonk-products-api-openapi.yml
  format: yaml
  label: ShipMonk Products API
  slug: shipmonk-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-products-api-openapi.yml
- filename: shipmonk-receivings-api-openapi.yml
  format: yaml
  label: ShipMonk Receivings API
  slug: shipmonk-receivings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-receivings-api-openapi.yml
- filename: shipmonk-returns-api-openapi.yml
  format: yaml
  label: ShipMonk Returns API
  slug: shipmonk-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-returns-api-openapi.yml
- filename: shipmonk-warehouses-api-openapi.yml
  format: yaml
  label: ShipMonk Warehouses API
  slug: shipmonk-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-warehouses-api-openapi.yml
- filename: shipmonk-webhooks-api-openapi.yml
  format: yaml
  label: ShipMonk Webhooks API
  slug: shipmonk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shipmonk Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShipMonk secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ShipMonk
provider_slug: shipmonk
scheme_count: 1
schemes:
- in: header
  name: api_key_header_Api-Key
  parameter: Api-Key
  sources:
  - openapi/shipmonk-orders-openapi.yml
  - openapi/shipmonk-products-openapi.yml
  - openapi/shipmonk-receivings-openapi.yml
  - openapi/shipmonk-returns-openapi.yml
  - openapi/shipmonk-warehouses-openapi.yml
  type: apiKey
slug: shipmonk-authentication
source_filename: shipmonk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/shipmonk-orders-openapi.yml, openapi/shipmonk-products-openapi.yml, openapi/shipmonk-receivings-openapi.yml,\n  openapi/shipmonk-returns-openapi.yml, openapi/shipmonk-warehouses-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key_header_Api-Key\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  sources:\n  - openapi/shipmonk-orders-openapi.yml\n  - openapi/shipmonk-products-openapi.yml\n  - openapi/shipmonk-receivings-openapi.yml\n  - openapi/shipmonk-returns-openapi.yml\n  - openapi/shipmonk-warehouses-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/authentication/shipmonk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Logistics
- Fulfillment
- 3PL
- E-Commerce
- Warehousing
- Inventory
- Shipping
- Returns
- Supply Chain
- Direct to Consumer
- Order Management
---
