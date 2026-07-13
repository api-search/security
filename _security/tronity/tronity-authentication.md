---
api_key_in: []
api_specs:
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Vehicles API
  slug: tronity-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Vehicle Data API
  slug: tronity-vehicle-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Charging & Battery API
  slug: tronity-charging-battery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Commands API
  slug: tronity-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Webhooks API
  slug: tronity-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tronity Authentication
name_suffix: Authentication
oauth_flows: []
overview: TRONITY secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TRONITY
provider_slug: tronity
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 Bearer access token obtained from POST /oauth/authentication. Available scopes include read_vin, read_vehicle_info, read_odometer, read_charge, read_battery, read_location, write_charge_start_stop and write_wake_up; the effective scope set is constrained by what the vehicle owner has granted.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tronity-openapi.yml
  type: http
slug: tronity-authentication
source_filename: tronity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tronity-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 Bearer access token obtained from POST /oauth/authentication. Available\n    scopes include read_vin, read_vehicle_info, read_odometer, read_charge, read_battery, read_location,\n    write_charge_start_stop and write_wake_up; the effective scope set is constrained by what\n    the vehicle owner has granted.\n  sources:\n  - openapi/tronity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/authentication/tronity-authentication.yml
summary_line: http · 1 scheme
tags:
- Connected Car
- EV
- Telematics
- Fleet
- Vehicle Data
---
