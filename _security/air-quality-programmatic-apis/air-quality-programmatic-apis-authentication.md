---
api_key_in:
- query
api_specs:
- filename: air-quality-programmatic-apis-air-quality-programmatic-apis-real-time-air-quality-tile-api-api-openapi.yml
  format: yaml
  label: Air Quality Programmatic APIs Air Quality Programmatic APIs Real Time Air Quality Tile API API
  slug: air-quality-programmatic-apis-air-quality-programmatic-apis-real-time-air-quality-tile-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/air-quality-programmatic-apis-air-quality-programmatic-apis-real-time-air-quality-tile-api-api-openapi.yml
- filename: air-quality-programmatic-apis-cities-api-openapi.yml
  format: yaml
  label: Air Quality Programmatic APIs Cities API
  slug: air-quality-programmatic-apis-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/air-quality-programmatic-apis-cities-api-openapi.yml
- filename: air-quality-programmatic-apis-geolocation-api-openapi.yml
  format: yaml
  label: Air Quality Programmatic APIs Geolocation API
  slug: air-quality-programmatic-apis-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/air-quality-programmatic-apis-geolocation-api-openapi.yml
- filename: air-quality-programmatic-apis-map-api-openapi.yml
  format: yaml
  label: Air Quality Programmatic APIs Map API
  slug: air-quality-programmatic-apis-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/air-quality-programmatic-apis-map-api-openapi.yml
- filename: air-quality-programmatic-apis-search-api-openapi.yml
  format: yaml
  label: Air Quality Programmatic APIs Search API
  slug: air-quality-programmatic-apis-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/air-quality-programmatic-apis-search-api-openapi.yml
- filename: air-quality-programmatic-apis-stations-api-openapi.yml
  format: yaml
  label: Air Quality Programmatic APIs Stations API
  slug: air-quality-programmatic-apis-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/air-quality-programmatic-apis-stations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Air Quality Programmatic Apis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Air Quality Programmatic APIs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
scheme_count: 1
schemes:
- description: API key for authentication
  in: query
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/air-quality-programmatic-apis-openapi.yml
  - openapi/aqicn-json-api-openapi.yaml
  type: apiKey
slug: air-quality-programmatic-apis-authentication
source_filename: air-quality-programmatic-apis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/air-quality-programmatic-apis-openapi.yml, openapi/aqicn-json-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: API key for authentication\n  sources:\n  - openapi/air-quality-programmatic-apis-openapi.yml\n  - openapi/aqicn-json-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/authentication/air-quality-programmatic-apis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
---
