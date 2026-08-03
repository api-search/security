---
api_key_in:
- header
api_specs:
- filename: cart-com-online-store-openapi-original.yml
  format: yaml
  label: Cart.com Online Store API
  slug: online-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cart-com/refs/heads/main/openapi/cart-com-online-store-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cart Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cart.com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cart.com
provider_slug: cart-com
scheme_count: 1
schemes:
- in: header
  name: X-AC-Auth-Token
  parameter: X-AC-Auth-Token
  sources:
  - openapi/cart-com-online-store-openapi-original.yml
  type: apiKey
slug: cart-com-authentication
source_filename: cart-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/cart-com-online-store-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-AC-Auth-Token\n  type: apiKey\n  in: header\n  parameter: X-AC-Auth-Token\n  sources:\n  - openapi/cart-com-online-store-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cart-com/refs/heads/main/authentication/cart-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- E-Commerce
- Retail
- Order Management
- Fulfillment
- Logistics
- Marketplaces
- Storefront
- Catalog
- Shipping
---
