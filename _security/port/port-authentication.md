---
api_key_in:
- header
api_specs:
- filename: port-openapi.yml
  format: yaml
  label: Port API
  slug: port
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Port Authentication
name_suffix: Authentication
oauth_flows: []
overview: Port secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Port
provider_slug: port
scheme_count: 1
schemes:
- in: header
  name: bearer
  parameter: Authorization
  sources:
  - openapi/port-openapi.yml
  type: apiKey
slug: port-authentication
source_filename: port-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/port-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/port-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/authentication/port-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automations
- Developer Portals
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Software Catalog
---
