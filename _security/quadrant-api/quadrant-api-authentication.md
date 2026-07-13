---
api_key_in:
- header
api_specs:
- filename: quadrant-api-openapi.json
  format: json
  label: Quadrant API
  slug: quadrant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadrant-api/main/openapi/quadrant-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Quadrant Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quadrant API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quadrant API
provider_slug: quadrant-api
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: API-Key
  sources:
  - openapi/quadrant-api-openapi.json
  type: apiKey
slug: quadrant-api-authentication
source_filename: quadrant-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quadrant-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: API-Key\n  sources:\n  - openapi/quadrant-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quadrant-api/refs/heads/main/authentication/quadrant-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alerts
- Security
- Threat Intelligence
---
