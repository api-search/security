---
api_key_in:
- header
api_specs:
- filename: optibus-operations-openapi.yml
  format: yaml
  label: Optibus Operations API
  slug: optibus-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optibus/refs/heads/main/openapi/optibus-operations-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Optibus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Optibus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Optibus
provider_slug: optibus
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/optibus-operations-openapi.yml
  type: apiKey
slug: optibus-authentication
source_filename: optibus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/optibus-operations-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/optibus-operations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optibus/refs/heads/main/authentication/optibus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Vertical Software
- Public Transportation
- Transit
- Scheduling
- Fleet Management
- Mobility
- Optimization
- Workforce Management
---
