---
api_key_in:
- query
api_specs:
- filename: wunderground-pws-api.yml
  format: yaml
  label: Weather Underground PWS API
  slug: weather-underground-pws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderground/refs/heads/main/openapi/wunderground-pws-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wunderground Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weather Underground secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weather Underground
provider_slug: wunderground
scheme_count: 1
schemes:
- description: API key issued to registered PWS contributors via https://www.wunderground.com/member/api-keys
  in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/wunderground-pws-api.yml
  type: apiKey
slug: wunderground-authentication
source_filename: wunderground-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wunderground-pws-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key issued to registered PWS contributors via https://www.wunderground.com/member/api-keys\n  sources:\n  - openapi/wunderground-pws-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderground/refs/heads/main/authentication/wunderground-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Personal Weather Stations
- Hyperlocal
- Observations
- Forecasts
- Historical Data
- REST API
---
