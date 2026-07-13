---
api_key_in:
- query
api_specs:
- filename: bls-public-data-api-openapi.yml
  format: yaml
  label: BLS Public Data API
  slug: bls-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bureau-of-labor-statistics/refs/heads/main/openapi/bls-public-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Us Bureau Of Labor Statistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: US Bureau of Labor Statistics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: US Bureau of Labor Statistics
provider_slug: us-bureau-of-labor-statistics
scheme_count: 1
schemes:
- description: Free API registration key from https://data.bls.gov/registrationEngine/. Required for v2 API access with higher rate limits.
  in: query
  name: ApiKey
  parameter: registrationkey
  sources:
  - openapi/bls-public-data-api-openapi.yml
  type: apiKey
slug: us-bureau-of-labor-statistics-authentication
source_filename: us-bureau-of-labor-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bls-public-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: registrationkey\n  description: Free API registration key from https://data.bls.gov/registrationEngine/. Required\n    for v2 API access with higher rate limits.\n  sources:\n  - openapi/bls-public-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-bureau-of-labor-statistics/refs/heads/main/authentication/us-bureau-of-labor-statistics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Labor Statistics
- Economic Data
- Open Data
---
