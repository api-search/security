---
api_key_in:
- query
api_specs:
- filename: openweather-openapi.yml
  format: yaml
  label: OpenWeather One Call API
  slug: openweather-one-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweather/refs/heads/main/openapi/openweather-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openweather Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenWeather secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenWeather
provider_slug: openweather
scheme_count: 1
schemes:
- in: query
  name: appid
  parameter: appid
  sources:
  - openapi/openweather-openapi.yml
  type: apiKey
slug: openweather-authentication
source_filename: openweather-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openweather-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: appid\n  type: apiKey\n  in: query\n  parameter: appid\n  sources:\n  - openapi/openweather-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweather/refs/heads/main/authentication/openweather-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Air Pollution
- Air Quality
- Climate
- Forecasting
- Weather
---
