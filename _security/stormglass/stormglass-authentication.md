---
api_key_in:
- header
api_specs:
- filename: stormglass-openapi.yml
  format: yaml
  label: Stormglass API
  slug: stormglass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stormglass/refs/heads/main/openapi/stormglass-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stormglass Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stormglass secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stormglass
provider_slug: stormglass
scheme_count: 1
schemes:
- description: API key obtained from your Stormglass account dashboard
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/stormglass-openapi.yml
  type: apiKey
slug: stormglass-authentication
source_filename: stormglass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stormglass-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key obtained from your Stormglass account dashboard\n  sources:\n  - openapi/stormglass-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stormglass/refs/heads/main/authentication/stormglass-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Astronomy
- Bio
- Climate
- Elevation
- Forecasting
- Marine
- Ocean
- Solar
- Tides
- Weather
- Wind
---
