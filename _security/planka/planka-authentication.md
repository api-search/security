---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Planka Authentication
name_suffix: Authentication
oauth_flows: []
overview: PLANKA secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PLANKA
provider_slug: planka
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/planka-openapi.json
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/planka-openapi.json
  type: apiKey
slug: planka-authentication
source_filename: planka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/planka-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/planka-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/planka-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/planka/authentication/planka-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Kanban
- Project Management
- Self-Hosted
- Agile
- Open Source
---
