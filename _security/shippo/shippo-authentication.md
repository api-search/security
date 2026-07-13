---
api_key_in: []
api_specs:
- filename: shippo-openapi.yml
  format: yaml
  label: Shippo API
  slug: shippo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shippo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shippo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shippo
provider_slug: shippo
scheme_count: 1
schemes:
- description: Shippo API token (prefix with "ShippoToken ")
  name: ShippoToken
  scheme: bearer
  sources:
  - openapi/shippo-openapi.yml
  type: http
slug: shippo-authentication
source_filename: shippo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shippo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ShippoToken\n  type: http\n  scheme: bearer\n  description: Shippo API token (prefix with \"ShippoToken \")\n  sources:\n  - openapi/shippo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/authentication/shippo-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Labels
- Logistics
- Returns
- Shipping
- Tracking
---
