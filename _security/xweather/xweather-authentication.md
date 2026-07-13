---
api_key_in:
- query
api_specs:
- filename: xweather-weather-api-openapi.yml
  format: yaml
  label: Xweather Weather API
  slug: xweather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-weather-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Xweather Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xweather secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xweather
provider_slug: xweather
scheme_count: 1
schemes:
- description: Xweather uses client_id and client_secret query parameters for authentication. Both are required on every request.
  in: query
  name: clientAuth
  parameter: client_id
  sources:
  - openapi/xweather-weather-api-openapi.yml
  type: apiKey
slug: xweather-authentication
source_filename: xweather-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xweather-weather-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: clientAuth\n  type: apiKey\n  in: query\n  parameter: client_id\n  description: Xweather uses client_id and client_secret query parameters for authentication.\n    Both are required on every request.\n  sources:\n  - openapi/xweather-weather-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/authentication/xweather-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Air Quality
- Company
- Data
- Forecasts
- Lightning
- Maritime
- Observations
- Severe Weather
- Weather
---
