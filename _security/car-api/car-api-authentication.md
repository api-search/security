---
api_key_in: []
api_specs:
- filename: car-api-openapi-original.yml
  format: yaml
  label: CarAPI Vehicle API
  slug: vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Car Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Car API (carapi.app) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Car API (carapi.app)
provider_slug: car-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/car-api-openapi-original.yml
  type: http
slug: car-api-authentication
source_filename: car-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/car-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/car-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/authentication/car-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Automobiles
- Automotive Data
- Cars
- License Plate Decoder
- OBD-II
- Power Sports
- Vehicle API
- Vehicle Specifications
- Vehicles
- VIN Decoder
---
