---
api_key_in: []
api_specs:
- filename: tictactrip-openapi-original.json
  format: json
  label: Tictactrip API
  slug: tictactrip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tictactrip Authentication
name_suffix: Authentication
oauth_flows: []
overview: TicTacTrip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TicTacTrip
provider_slug: tictactrip
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: authentication
  scheme: bearer
  sources:
  - openapi/tictactrip-openapi-original.json
  type: http
slug: tictactrip-authentication
source_filename: tictactrip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tictactrip-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: authentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tictactrip-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/authentication/tictactrip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Travel
- Transportation
- Trains
- Buses
- Booking
- Mobility
- Multimodal
- Ticketing
---
