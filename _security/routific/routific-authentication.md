---
api_key_in: []
api_specs:
- filename: routific-route-optimization-api-openapi.yml
  format: yaml
  label: Routific Route Optimization API
  slug: routific-route-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/openapi/routific-route-optimization-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Routific Authentication
name_suffix: Authentication
oauth_flows: []
overview: Routific secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Routific
provider_slug: routific
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Routific issues per-account JWT tokens. Send as

    `Authorization: bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/routific-route-optimization-api-openapi.yml
  type: http
slug: routific-authentication
source_filename: routific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/routific-route-optimization-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Routific issues per-account JWT tokens. Send as\n    `Authorization: bearer <token>`.\n  sources:\n  - openapi/routific-route-optimization-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/authentication/routific-authentication.yml
summary_line: http · 1 scheme
tags:
- RouteOptimization
- VRP
- PickupAndDelivery
- Logistics
- LastMileDelivery
- Delivery
- FleetManagement
- Dispatch
- DeliveryManagement
---
