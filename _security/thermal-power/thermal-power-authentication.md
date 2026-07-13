---
api_key_in:
- query
api_specs:
- filename: thermal-power-openapi.yml
  format: yaml
  label: Thermal Power API
  slug: thermal-power
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermal-power/refs/heads/main/openapi/thermal-power-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Thermal Power Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thermal Power secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Thermal Power
provider_slug: thermal-power
scheme_count: 1
schemes:
- description: EIA API key. Register for free at https://www.eia.gov/opendata/register.php
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/thermal-power-openapi.yml
  type: apiKey
slug: thermal-power-authentication
source_filename: thermal-power-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thermal-power-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: EIA API key. Register for free at https://www.eia.gov/opendata/register.php\n  sources:\n  - openapi/thermal-power-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thermal-power/refs/heads/main/authentication/thermal-power-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Thermal Power
- Power Generation
- Electricity
- Coal
- Natural Gas
- Nuclear
---
