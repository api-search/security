---
api_key_in: []
api_specs:
- filename: cargoson-carriers-api-openapi.yml
  format: yaml
  label: Cargoson Carriers API
  slug: cargoson-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-carriers-api-openapi.yml
- filename: cargoson-price-requests-api-openapi.yml
  format: yaml
  label: Cargoson Price Requests API
  slug: cargoson-price-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-price-requests-api-openapi.yml
- filename: cargoson-shipments-api-openapi.yml
  format: yaml
  label: Cargoson Shipments API
  slug: cargoson-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-shipments-api-openapi.yml
- filename: cargoson-transports-tracking-api-openapi.yml
  format: yaml
  label: Cargoson Transports & Tracking API
  slug: cargoson-transports-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-transports-tracking-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cargoson Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cargoson secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cargoson
provider_slug: cargoson
scheme_count: 1
schemes:
- description: 'API key passed as a Bearer token in the Authorization header (`Authorization: Bearer [example key]`). Requests must also send `Accept: application/vnd.api.v1`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cargoson-openapi.yml
  type: http
slug: cargoson-authentication
source_filename: cargoson-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cargoson-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key passed as a Bearer token in the Authorization header (`Authorization:\n    Bearer [example key]`). Requests must also send `Accept: application/vnd.api.v1`.'\n  sources:\n  - openapi/cargoson-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/authentication/cargoson-authentication.yml
summary_line: http · 1 scheme
tags:
- Transport Management
- TMS
- Freight
- Shipping
- Logistics
- Carriers
---
