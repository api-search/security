---
api_key_in: []
api_specs:
- filename: meteomatics-weather-openapi.yml
  format: yaml
  label: Meteomatics Weather API
  slug: meteomatics-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meteomatics/refs/heads/main/openapi/meteomatics-weather-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Meteomatics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meteomatics secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Meteomatics
provider_slug: meteomatics
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using Meteomatics account credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/meteomatics-weather-openapi.yml
  type: http
- bearerFormat: JWT
  description: JWT bearer token obtained from `https://login.meteomatics.com/api/v1/token`. May also be supplied as the `access_token` query parameter.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/meteomatics-weather-openapi.yml
  type: http
slug: meteomatics-authentication
source_filename: meteomatics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meteomatics-weather-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Meteomatics account credentials.\n  sources:\n  - openapi/meteomatics-weather-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token obtained from `https://login.meteomatics.com/api/v1/token`.\n    May also be supplied as the `access_token` query parameter.\n  sources:\n  - openapi/meteomatics-weather-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meteomatics/refs/heads/main/authentication/meteomatics-authentication.yml
summary_line: http · 2 schemes
tags:
- Weather
- Forecast
- Climate
- Historical Weather
- Marine
- Environmental Data
- Hyperlocal
- Meteorology
- Time Series
- Geospatial
---
