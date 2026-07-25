---
api_key_in: []
api_specs:
- filename: shipbob-subpackage-billing-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_billing API
  slug: shipbob-subpackage-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-billing-api-openapi.yml
- filename: shipbob-subpackage-channels-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_channels API
  slug: shipbob-subpackage-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-channels-api-openapi.yml
- filename: shipbob-subpackage-inventory-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_inventory API
  slug: shipbob-subpackage-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-inventory-api-openapi.yml
- filename: shipbob-subpackage-locations-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_locations API
  slug: shipbob-subpackage-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-locations-api-openapi.yml
- filename: shipbob-subpackage-orders-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_orders API
  slug: shipbob-subpackage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-orders-api-openapi.yml
- filename: shipbob-subpackage-products-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_products API
  slug: shipbob-subpackage-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-products-api-openapi.yml
- filename: shipbob-subpackage-receiving-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_receiving API
  slug: shipbob-subpackage-receiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-receiving-api-openapi.yml
- filename: shipbob-subpackage-returns-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_returns API
  slug: shipbob-subpackage-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-returns-api-openapi.yml
- filename: shipbob-subpackage-simulations-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_simulations API
  slug: shipbob-subpackage-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-simulations-api-openapi.yml
- filename: shipbob-subpackage-webhooks-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_webhooks API
  slug: shipbob-subpackage-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shipbob Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShipBob secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ShipBob
provider_slug: shipbob
scheme_count: 1
schemes:
- description: Authentication using Personal Access Token (PAT) token or OAuth2
  name: PAT
  scheme: bearer
  sources:
  - openapi/shipbob-openapi.json
  type: http
slug: shipbob-authentication
source_filename: shipbob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shipbob-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: PAT\n  type: http\n  scheme: bearer\n  description: Authentication using Personal Access Token (PAT) token or OAuth2\n  sources:\n  - openapi/shipbob-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/authentication/shipbob-authentication.yml
summary_line: http · 1 scheme
tags:
- Logistics
- Fulfillment
- 3PL
- Ecommerce
- Inventory
- Warehousing
- Shipping
- Direct-to-Consumer
---
