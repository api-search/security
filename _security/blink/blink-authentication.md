---
api_key_in:
- query
api_specs:
- filename: blink-charging-locations-status-openapi.yml
  format: yaml
  label: Blink Charging Locations & Status API
  slug: blink-charging-locations-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blink/refs/heads/main/openapi/blink-charging-locations-status-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blink Charging secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blink Charging
provider_slug: blink
scheme_count: 1
schemes:
- description: API key issued after signing up for Blink's third-party integrator program. Exact transport (query parameter vs. header) is not independently re-verified for the current API version.
  in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/blink-charging-locations-status-openapi.yml
  type: apiKey
slug: blink-authentication
source_filename: blink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blink-charging-locations-status-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key issued after signing up for Blink's third-party integrator program. Exact\n    transport (query parameter vs. header) is not independently re-verified for the current\n    API version.\n  sources:\n  - openapi/blink-charging-locations-status-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blink/refs/heads/main/authentication/blink-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- EV Charging
- Electric Vehicle
- Charging Stations
- OCPI
- OCPP
- Fleet Management
- Roaming
- DC Fast Charging
---
