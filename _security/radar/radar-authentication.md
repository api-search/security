---
api_key_in:
- header
api_specs:
- filename: radar-openapi.yml
  format: yaml
  label: Radar
  slug: radar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/openapi/radar-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Radar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Radar
provider_slug: radar
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/radar-openapi.yml
  type: apiKey
slug: radar-authentication
source_filename: radar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/radar-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/radar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radar/refs/heads/main/authentication/radar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Location
- Geocoding
- Geofencing
- Routing
- Maps
---
