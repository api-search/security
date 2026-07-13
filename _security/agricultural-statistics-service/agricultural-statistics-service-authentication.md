---
api_key_in:
- query
api_specs:
- filename: agricultural-statistics-service-quickstats-api.yaml
  format: yaml
  label: USDA NASS QuickStats API
  slug: quickstats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/openapi/agricultural-statistics-service-quickstats-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agricultural Statistics Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agricultural Statistics Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
scheme_count: 1
schemes:
- description: API key obtained by registering at https://quickstats.nass.usda.gov/api and agreeing to NASS Terms of Service.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/agricultural-statistics-service-quickstats-api.yaml
  type: apiKey
slug: agricultural-statistics-service-authentication
source_filename: agricultural-statistics-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agricultural-statistics-service-quickstats-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key obtained by registering at https://quickstats.nass.usda.gov/api and agreeing\n    to NASS Terms of Service.\n  sources:\n  - openapi/agricultural-statistics-service-quickstats-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/authentication/agricultural-statistics-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
---
