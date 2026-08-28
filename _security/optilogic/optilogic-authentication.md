---
api_key_in:
- header
api_specs:
- filename: optilogic-rest-api-openapi.json
  format: json
  label: Optilogic REST API
  slug: optilogic-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-rest-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Optilogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Optilogic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Optilogic
provider_slug: optilogic
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/optilogic-rest-api-openapi.json
  type: apiKey
slug: optilogic-authentication
source_filename: optilogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/optilogic-rest-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/optilogic-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/authentication/optilogic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Supply Chain
- Supply Chain Design
- Network Optimization
- Simulation
- Optimization
- Logistics
- Analytics
- Artificial Intelligence
- Jobs
- Cloud
---
