---
api_key_in:
- query
api_specs:
- filename: airvisual-cities-api-openapi.yml
  format: yaml
  label: IQAir AirVisual Cities API
  slug: airvisual-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/openapi/airvisual-cities-api-openapi.yml
- filename: airvisual-countries-api-openapi.yml
  format: yaml
  label: IQAir AirVisual Countries API
  slug: airvisual-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/openapi/airvisual-countries-api-openapi.yml
- filename: airvisual-rankings-api-openapi.yml
  format: yaml
  label: IQAir AirVisual Rankings API
  slug: airvisual-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/openapi/airvisual-rankings-api-openapi.yml
- filename: airvisual-states-api-openapi.yml
  format: yaml
  label: IQAir AirVisual States API
  slug: airvisual-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/openapi/airvisual-states-api-openapi.yml
- filename: airvisual-stations-api-openapi.yml
  format: yaml
  label: IQAir AirVisual Stations API
  slug: airvisual-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/openapi/airvisual-stations-api-openapi.yml
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
