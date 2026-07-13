---
api_key_in:
- query
api_specs:
- filename: bls-public-data-api-openapi.yaml
  format: yaml
  label: BLS Public Data API
  slug: bls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-bureau-of-labor-statistics/refs/heads/main/openapi/bls-public-data-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: U S Bureau Of Labor Statistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: U.S. Bureau of Labor Statistics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: U.S. Bureau of Labor Statistics
provider_slug: u-s-bureau-of-labor-statistics
scheme_count: 1
schemes:
- description: Free BLS API registration key. Register at https://data.bls.gov/registrationEngine/ to obtain a key for Version 2 API features.
  in: query
  name: ApiKeyQuery
  parameter: registrationkey
  sources:
  - openapi/bls-public-data-api-openapi.yaml
  type: apiKey
slug: u-s-bureau-of-labor-statistics-authentication
source_filename: u-s-bureau-of-labor-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bls-public-data-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: registrationkey\n  description: Free BLS API registration key. Register at https://data.bls.gov/registrationEngine/\n    to obtain a key for Version 2 API features.\n  sources:\n  - openapi/bls-public-data-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/u-s-bureau-of-labor-statistics/refs/heads/main/authentication/u-s-bureau-of-labor-statistics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Labor
- Statistics
- Employment
- Economic Data
---
