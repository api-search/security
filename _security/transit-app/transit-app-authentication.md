---
api_key_in:
- header
api_specs:
- filename: transit-openapi.yml
  format: yaml
  label: Transit API
  slug: transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit-app/refs/heads/main/openapi/transit-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Transit App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transit
provider_slug: transit-app
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/transit-openapi.yml
  type: apiKey
slug: transit-app-authentication
source_filename: transit-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/transit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  sources:\n  - openapi/transit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transit-app/refs/heads/main/authentication/transit-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Transit
- Public Transit
- Multimodal
- Mobility
- Trip Planning
- Routing
- Real-Time
- GTFS
- GOFS
- Bikeshare
- Scooters
- Carshare
- On-Demand Transit
- Service Alerts
- Shared Mobility
- Crowdsourced Data
---
