---
api_key_in:
- query
api_specs:
- filename: eia-open-data-api-openapi.yaml
  format: yaml
  label: EIA Open Data API
  slug: eia-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/eia-open-data-api-openapi.yaml
- filename: docs
  format: yaml
  label: OSTI.GOV API
  slug: osti-api
  spec_type: OpenAPI
  url: https://www.osti.gov/api/v1/docs
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Doe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Energy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of Energy
provider_slug: doe
scheme_count: 1
schemes:
- in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/eia-open-data-api-openapi.yaml
  type: apiKey
slug: doe-authentication
source_filename: doe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eia-open-data-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/eia-open-data-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/authentication/doe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Government
- Renewable Energy
- Electricity
- Natural Gas
- Petroleum
- Solar
- Wind
- Electric Vehicles
- Alternative Fuels
- Nuclear
- Scientific Research
---
