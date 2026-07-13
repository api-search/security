---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: SolarEdge Monitoring API
  slug: solar-edge-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Solar Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: SolarEdge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SolarEdge
provider_slug: solar-edge
scheme_count: 1
schemes:
- description: API key generated through the SolarEdge monitoring portal
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/solar-edge-monitoring-api-openapi.yml
  type: apiKey
slug: solar-edge-authentication
source_filename: solar-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/solar-edge-monitoring-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key generated through the SolarEdge monitoring portal\n  sources:\n  - openapi/solar-edge-monitoring-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/authentication/solar-edge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Solar
- Energy
- Monitoring
- PV
- Inverter
- Renewable Energy
- IoT
---
