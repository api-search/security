---
api_key_in: []
api_specs:
- filename: routific-fix-api-openapi.yml
  format: yaml
  label: Routific Fix API
  slug: routific-fix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/openapi/routific-fix-api-openapi.yml
- filename: routific-jobs-api-openapi.yml
  format: yaml
  label: Routific Jobs API
  slug: routific-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/openapi/routific-jobs-api-openapi.yml
- filename: routific-pdp-api-openapi.yml
  format: yaml
  label: Routific PDP API
  slug: routific-pdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/openapi/routific-pdp-api-openapi.yml
- filename: routific-vrp-api-openapi.yml
  format: yaml
  label: Routific VRP API
  slug: routific-vrp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/openapi/routific-vrp-api-openapi.yml
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
- Route Optimization
- VRP
- Pickup and Delivery
- Logistics
- Last Mile Delivery
- Delivery
- Fleet Management
- Dispatch
- Delivery Management
---
