---
api_key_in:
- header
api_specs:
- filename: vehicle-databases-openapi.yml
  format: yaml
  label: Vehicle Databases Maintenance API
  slug: vehicle-databases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-databases/refs/heads/main/openapi/vehicle-databases-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vehicle Databases Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vehicle Databases secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vehicle Databases
provider_slug: vehicle-databases
scheme_count: 1
schemes:
- description: Vehicle Databases API key
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/vehicle-databases-openapi.yml
  type: apiKey
slug: vehicle-databases-authentication
source_filename: vehicle-databases-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vehicle-databases-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Vehicle Databases API key\n  sources:\n  - openapi/vehicle-databases-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vehicle-databases/refs/heads/main/authentication/vehicle-databases-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- Fleet Management
- Maintenance
- Recalls
- Vehicles
---
