---
api_key_in:
- header
- query
api_specs:
- filename: bls-surveys-api-openapi.yml
  format: yaml
  label: Bureau of Labor Statistics Surveys API
  slug: bls-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bls/refs/heads/main/openapi/bls-surveys-api-openapi.yml
- filename: bls-time-series-api-openapi.yml
  format: yaml
  label: Bureau of Labor Statistics Time Series API
  slug: bls-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bls/refs/heads/main/openapi/bls-time-series-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bls Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Labor Statistics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bureau of Labor Statistics
provider_slug: bls
scheme_count: 2
schemes:
- description: BLS API registration key. Required for Version 2.0 features (catalog metadata, calculations, annual averages, higher rate limits). Obtain for free at https://data.bls.gov/registrationEngine/.
  in: query
  name: apiKeyQuery
  parameter: registrationkey
  sources:
  - openapi/bls-public-data-api-openapi.yml
  type: apiKey
- description: BLS API registration key passed in the JSON request body for POST requests.
  in: header
  name: apiKeyBody
  parameter: registrationkey
  sources:
  - openapi/bls-public-data-api-openapi.yml
  type: apiKey
slug: bls-authentication
source_filename: bls-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bls-public-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: registrationkey\n  description: BLS API registration key. Required for Version 2.0 features (catalog metadata,\n    calculations, annual averages, higher rate limits). Obtain for free at https://data.bls.gov/registrationEngine/.\n  sources:\n  - openapi/bls-public-data-api-openapi.yml\n- name: apiKeyBody\n  type: apiKey\n  in: header\n  parameter: registrationkey\n  description: BLS API registration key passed in the JSON request body for POST requests.\n  sources:\n  - openapi/bls-public-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bls/refs/heads/main/authentication/bls-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Bureau of Labor Statistics
- BLS
- Employment
- Unemployment
- CPI
- Consumer Price Index
- PPI
- Producer Price Index
- Wages
- Labor Statistics
- Economic Indicators
- Federal-Government
- Open Data
---
