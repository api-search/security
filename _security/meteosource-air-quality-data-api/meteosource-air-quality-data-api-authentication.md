---
api_key_in:
- header
- query
api_specs:
- filename: meteosource-air-quality-data-api-openapi.yml
  format: yaml
  label: MeteoSource Air Quality Data API
  slug: meteosource-air-quality-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meteosource-air-quality-data-api/refs/heads/main/openapi/meteosource-air-quality-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Meteosource Air Quality Data Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: MeteoSource Air Quality Data API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MeteoSource Air Quality Data API
provider_slug: meteosource-air-quality-data-api
scheme_count: 2
schemes:
- in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/meteosource-air-quality-data-api-openapi.yml
  type: apiKey
- in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/meteosource-air-quality-data-api-openapi.yml
  type: apiKey
slug: meteosource-air-quality-data-api-authentication
source_filename: meteosource-air-quality-data-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meteosource-air-quality-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/meteosource-air-quality-data-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/meteosource-air-quality-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meteosource-air-quality-data-api/refs/heads/main/authentication/meteosource-air-quality-data-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Air Quality
- Environmental Data
- Forecasting
- Weather
---
