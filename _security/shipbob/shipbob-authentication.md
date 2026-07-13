---
api_key_in: []
api_specs:
- filename: shipbob-openapi.json
  format: json
  label: ShipBob Developer API
  slug: shipbob-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-openapi.json
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
