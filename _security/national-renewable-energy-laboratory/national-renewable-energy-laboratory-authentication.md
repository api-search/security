---
api_key_in:
- query
api_specs:
- filename: national-renewable-energy-laboratory-openapi.yml
  format: yaml
  label: NREL Developer Network
  slug: nrel-developer-network
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-renewable-energy-laboratory/refs/heads/main/openapi/national-renewable-energy-laboratory-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: National Renewable Energy Laboratory Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Renewable Energy Laboratory secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Renewable Energy Laboratory
provider_slug: national-renewable-energy-laboratory
scheme_count: 1
schemes:
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/national-renewable-energy-laboratory-openapi.yml
  type: apiKey
slug: national-renewable-energy-laboratory-authentication
source_filename: national-renewable-energy-laboratory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/national-renewable-energy-laboratory-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/national-renewable-energy-laboratory-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-renewable-energy-laboratory/refs/heads/main/authentication/national-renewable-energy-laboratory-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Renewable Energy
- Federal Government
- Climate
- Research
---
