---
api_key_in:
- header
api_specs:
- filename: padlet-openapi.yml
  format: yaml
  label: Padlet API
  slug: padlet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/padlet/refs/heads/main/openapi/padlet-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Padlet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Padlet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Padlet
provider_slug: padlet
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/padlet-openapi.yml
  type: apiKey
slug: padlet-authentication
source_filename: padlet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/padlet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/padlet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/padlet/refs/heads/main/authentication/padlet-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Collaboration
- Education
- Visual Collaboration
- Content
- Boards
- Productivity
- JSON:API
- MCP
- EdTech
---
