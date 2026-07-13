---
api_key_in:
- header
api_specs:
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Orders API
  slug: gelato-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Product Catalog API
  slug: gelato-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Prices and Stock API
  slug: gelato-prices-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Shipment API
  slug: gelato-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Ecommerce API
  slug: gelato-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Webhooks API
  slug: gelato-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gelato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gelato secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gelato
provider_slug: gelato
scheme_count: 1
schemes:
- description: Gelato API key passed in the X-API-KEY header on every request. All requests must be made over HTTPS.
  in: header
  name: api_key
  parameter: X-API-KEY
  sources:
  - openapi/gelato-openapi.yml
  type: apiKey
slug: gelato-authentication
source_filename: gelato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gelato-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Gelato API key passed in the X-API-KEY header on every request. All requests\n    must be made over HTTPS.\n  sources:\n  - openapi/gelato-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/authentication/gelato-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Print on Demand
- Ecommerce
- Fulfillment
- Distributed Production
- Orders
---
