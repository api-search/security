---
api_key_in:
- header
api_specs:
- filename: transit-openapi.yml
  format: yaml
  label: Transit API
  slug: transit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Transit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transit
provider_slug: transit
scheme_count: 1
schemes:
- description: API key provided after partner approval
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/transit-openapi.yml
  type: apiKey
slug: transit-authentication
source_filename: transit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/transit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key provided after partner approval\n  sources:\n  - openapi/transit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/authentication/transit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Public Transit
- Real-Time
- Trip Planning
- Multimodal
- GTFS
- GOFS
- Mobility
- Shared Mobility
---
