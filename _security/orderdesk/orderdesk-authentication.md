---
api_key_in:
- header
api_specs:
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Orders API
  slug: orderdesk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Order Items API
  slug: orderdesk-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Shipments API
  slug: orderdesk-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Inventory Items API
  slug: orderdesk-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Store API
  slug: orderdesk-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Orderdesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Order Desk secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Order Desk
provider_slug: orderdesk
scheme_count: 2
schemes:
- description: The numeric ID of your Order Desk store.
  in: header
  name: storeId
  parameter: ORDERDESK-STORE-ID
  sources:
  - openapi/orderdesk-openapi.yml
  type: apiKey
- description: The API key for your Order Desk store.
  in: header
  name: apiKey
  parameter: ORDERDESK-API-KEY
  sources:
  - openapi/orderdesk-openapi.yml
  type: apiKey
slug: orderdesk-authentication
source_filename: orderdesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orderdesk-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: storeId\n  type: apiKey\n  in: header\n  parameter: ORDERDESK-STORE-ID\n  description: The numeric ID of your Order Desk store.\n  sources:\n  - openapi/orderdesk-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: ORDERDESK-API-KEY\n  description: The API key for your Order Desk store.\n  sources:\n  - openapi/orderdesk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/authentication/orderdesk-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Ecommerce
- Order Management
- Fulfillment
- Dropshipping
- Inventory
- Shipping
---
