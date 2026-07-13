---
api_key_in:
- header
api_specs:
- filename: windy-openapi.yml
  format: yaml
  label: Windy Point Forecast API
  slug: point-forecast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-openapi.yml
- filename: windy-openapi.yml
  format: yaml
  label: Windy Map Forecast API
  slug: map-forecast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-openapi.yml
- filename: windy-openapi.yml
  format: yaml
  label: Windy Webcams API
  slug: webcams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Windy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Windy
provider_slug: windy
scheme_count: 1
schemes:
- description: Windy Webcams API key, obtained at https://api.windy.com/keys.
  in: header
  name: WindyApiKey
  parameter: x-windy-api-key
  sources:
  - openapi/windy-openapi.yml
  type: apiKey
slug: windy-authentication
source_filename: windy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/windy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: WindyApiKey\n  type: apiKey\n  in: header\n  parameter: x-windy-api-key\n  description: Windy Webcams API key, obtained at https://api.windy.com/keys.\n  sources:\n  - openapi/windy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/authentication/windy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Forecast
- Maps
- Webcams
- Visualization
---
