---
api_key_in:
- query
api_specs:
- filename: tomorrow-openapi.yml
  format: yaml
  label: Tomorrow.io Weather API
  slug: tomorrowio-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/openapi/tomorrow-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tomorrow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tomorrow.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tomorrow.io
provider_slug: tomorrow
scheme_count: 1
schemes:
- description: Tomorrow.io API key passed as `apikey` query parameter. Obtain at https://app.tomorrow.io/development/keys.
  in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/tomorrow-openapi.yml
  type: apiKey
slug: tomorrow-authentication
source_filename: tomorrow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tomorrow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Tomorrow.io API key passed as `apikey` query parameter. Obtain at https://app.tomorrow.io/development/keys.\n  sources:\n  - openapi/tomorrow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomorrow/refs/heads/main/authentication/tomorrow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Climate
- Forecast
- Historical Weather
- Air Quality
- Pollen
- Fire
- Flood
- Routes
- Map Tiles
- Aviation
- Maritime
- Public APIs
---
