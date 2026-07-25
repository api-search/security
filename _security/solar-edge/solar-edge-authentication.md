---
api_key_in:
- query
api_specs:
- filename: solar-edge-accounts-api-openapi.yml
  format: yaml
  label: SolarEdge Accounts API
  slug: solar-edge-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-accounts-api-openapi.yml
- filename: solar-edge-energy-api-openapi.yml
  format: yaml
  label: SolarEdge Energy API
  slug: solar-edge-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-energy-api-openapi.yml
- filename: solar-edge-environmental-api-openapi.yml
  format: yaml
  label: SolarEdge Environmental API
  slug: solar-edge-environmental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-environmental-api-openapi.yml
- filename: solar-edge-equipment-api-openapi.yml
  format: yaml
  label: SolarEdge Equipment API
  slug: solar-edge-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-equipment-api-openapi.yml
- filename: solar-edge-power-api-openapi.yml
  format: yaml
  label: SolarEdge Power API
  slug: solar-edge-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-power-api-openapi.yml
- filename: solar-edge-sites-api-openapi.yml
  format: yaml
  label: SolarEdge Sites API
  slug: solar-edge-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-sites-api-openapi.yml
- filename: solar-edge-storage-api-openapi.yml
  format: yaml
  label: SolarEdge Storage API
  slug: solar-edge-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-storage-api-openapi.yml
- filename: solar-edge-version-api-openapi.yml
  format: yaml
  label: SolarEdge Version API
  slug: solar-edge-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solar-edge/refs/heads/main/openapi/solar-edge-version-api-openapi.yml
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
