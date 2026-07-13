---
api_key_in:
- query
api_specs:
- filename: department-of-energy-openapi.yml
  format: yaml
  label: EIA Open Data API V2
  slug: eia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Department Of Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Energy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of Energy
provider_slug: department-of-energy
scheme_count: 1
schemes:
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/department-of-energy-openapi.yml
  type: apiKey
slug: department-of-energy-authentication
source_filename: department-of-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/department-of-energy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/department-of-energy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/authentication/department-of-energy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Buildings
- Electricity
- Energy
- Federal Government
- Open Data
- Renewables
- Research
- Solar
- Statistics
---
