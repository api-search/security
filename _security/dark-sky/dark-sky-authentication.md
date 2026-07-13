---
api_key_in:
- path
api_specs:
- filename: openapi.yml
  format: yaml
  label: Dark Sky Forecast API
  slug: dark-sky-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dark-sky/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dark Sky Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dark Sky secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dark Sky
provider_slug: dark-sky
scheme_count: 1
schemes:
- description: Dark Sky API key included as the first path segment after /forecast/. Obtain your key from https://darksky.net/dev.
  in: path
  name: ApiKeyPath
  parameter: key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: dark-sky-authentication
source_filename: dark-sky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\nschemes:\n- name: ApiKeyPath\n  type: apiKey\n  in: path\n  parameter: key\n  description: Dark Sky API key included as the first path segment after /forecast/. Obtain\n    your key from https://darksky.net/dev.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dark-sky/refs/heads/main/authentication/dark-sky-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Forecast
- Hyperlocal
- Precipitation
- Machine Learning
- REST
- Apple
---
