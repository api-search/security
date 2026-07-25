---
api_key_in:
- query
api_specs:
- filename: waqi-feed-api-openapi.yml
  format: yaml
  label: World Air Quality Index (WAQI) Feed API
  slug: waqi-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waqi/refs/heads/main/openapi/waqi-feed-api-openapi.yml
- filename: waqi-map-api-openapi.yml
  format: yaml
  label: World Air Quality Index (WAQI) Map API
  slug: waqi-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waqi/refs/heads/main/openapi/waqi-map-api-openapi.yml
- filename: waqi-search-api-openapi.yml
  format: yaml
  label: World Air Quality Index (WAQI) Search API
  slug: waqi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waqi/refs/heads/main/openapi/waqi-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Waqi Authentication
name_suffix: Authentication
oauth_flows: []
overview: World Air Quality Index (WAQI) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: World Air Quality Index (WAQI)
provider_slug: waqi
scheme_count: 1
schemes:
- description: API token obtained from the Air Quality Open Data Platform at https://aqicn.org/data-platform/token/
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/waqi-openapi.json
  type: apiKey
slug: waqi-authentication
source_filename: waqi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/waqi-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token obtained from the Air Quality Open Data Platform at https://aqicn.org/data-platform/token/\n  sources:\n  - openapi/waqi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waqi/refs/heads/main/authentication/waqi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Air Quality
- AQI
- Environment
- Pollution
- Real-Time Data
- Weather
- IoT
- Open Data
---
