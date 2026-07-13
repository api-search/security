---
api_key_in:
- query
api_specs:
- filename: weatherapi-openapi-original.yml
  format: yaml
  label: WeatherAPI
  slug: weatherapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherapi/refs/heads/main/openapi/weatherapi-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Weatherapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeatherAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WeatherAPI
provider_slug: weatherapi
scheme_count: 1
schemes:
- description: API key obtained from https://www.weatherapi.com/my/. Pass as `?key=YOUR_API_KEY` query parameter.
  in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/weatherapi-openapi-original.yml
  type: apiKey
slug: weatherapi-authentication
source_filename: weatherapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weatherapi-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key obtained from https://www.weatherapi.com/my/. Pass as `?key=YOUR_API_KEY`\n    query parameter.\n  sources:\n  - openapi/weatherapi-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherapi/refs/heads/main/authentication/weatherapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Forecast
- History
- Marine
- Astronomy
- Geolocation
- Sports
- Alerts
- Public APIs
---
