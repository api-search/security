---
api_key_in:
- header
api_specs:
- filename: shortcut-software-openapi-original.json
  format: json
  label: Shortcut API
  slug: shortcut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut-software/refs/heads/main/openapi/shortcut-software-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shortcut Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shortcut Software secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shortcut Software
provider_slug: shortcut-software
scheme_count: 1
schemes:
- in: header
  name: api_token
  parameter: Shortcut-Token
  sources:
  - openapi/shortcut-software-openapi-original.json
  type: apiKey
slug: shortcut-software-authentication
source_filename: shortcut-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/shortcut-software-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_token\n  type: apiKey\n  in: header\n  parameter: Shortcut-Token\n  sources:\n  - openapi/shortcut-software-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortcut-software/refs/heads/main/authentication/shortcut-software-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Project Management
- Issue Tracking
- Agile
- Developer Tools
- Software Development
- Sprints
- Roadmaps
---
