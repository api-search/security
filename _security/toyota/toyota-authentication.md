---
api_key_in: []
api_specs:
- filename: toyota-vehicle-openapi.yml
  format: yaml
  label: Toyota Vehicle API
  slug: toyota-vehicle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-vehicle-openapi.yml
- filename: toyota-telematics-openapi.yml
  format: yaml
  label: Toyota Telematics API
  slug: toyota-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-telematics-openapi.yml
- filename: toyota-connected-services-openapi.yml
  format: yaml
  label: Toyota Connected Services API
  slug: toyota-connected-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-connected-services-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Toyota Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toyota secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Toyota
provider_slug: toyota
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/toyota-connected-services-openapi.yml
  - openapi/toyota-telematics-openapi.yml
  type: http
slug: toyota-authentication
source_filename: toyota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toyota-connected-services-openapi.yml, openapi/toyota-telematics-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/toyota-connected-services-openapi.yml\n  - openapi/toyota-telematics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/authentication/toyota-authentication.yml
summary_line: http · 1 scheme
tags:
- Automobiles
- Cars
- Vehicles
- Connected Car
- Telematics
- Fleet Management
- Electric Vehicles
---
