---
api_key_in:
- query
api_specs:
- filename: openapi.json
  format: json
  label: IQAir AirVisual API
  slug: iqair-airvisual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Airvisual Authentication
name_suffix: Authentication
oauth_flows: []
overview: IQAir AirVisual secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IQAir AirVisual
provider_slug: airvisual
scheme_count: 1
schemes:
- description: API key passed as a query parameter.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/openapi.json
  type: apiKey
slug: airvisual-authentication
source_filename: airvisual-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key passed as a query parameter.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/authentication/airvisual-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Air Quality
- AQI
- PM2.5
- Weather
- Pollution
- Environmental Data
- Real-Time Data
---
