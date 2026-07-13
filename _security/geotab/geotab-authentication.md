---
api_key_in: []
api_specs:
- filename: geotab-data-intake-gateway-openapi.yml
  format: yaml
  label: Data Intake Gateway API
  slug: data-intake-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geotab/refs/heads/main/openapi/geotab-data-intake-gateway-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Geotab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geotab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Geotab
provider_slug: geotab
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/geotab-data-intake-gateway-openapi.yml
  type: http
slug: geotab-authentication
source_filename: geotab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/geotab-data-intake-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/geotab-data-intake-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geotab/refs/heads/main/authentication/geotab-authentication.yml
summary_line: http · 1 scheme
tags:
- Fleet Management
- Telematics
- Vehicle Tracking
- ELD Compliance
- Driver Behavior
- Fuel Monitoring
- Route Optimization
- GPS Tracking
- IoT
---
