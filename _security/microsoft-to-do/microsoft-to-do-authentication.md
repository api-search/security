---
api_key_in: []
api_specs:
- filename: microsoft-to-do-openapi.yml
  format: yaml
  label: Microsoft Graph to Do Tasks API
  slug: graph-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-to-do/refs/heads/main/openapi/microsoft-to-do-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft To Do Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft to Do secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft to Do
provider_slug: microsoft-to-do
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-to-do-openapi.yml
  type: http
slug: microsoft-to-do-authentication
source_filename: microsoft-to-do-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-to-do-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-to-do-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-to-do/refs/heads/main/authentication/microsoft-to-do-authentication.yml
summary_line: http · 1 scheme
tags:
- Microsoft
- Microsoft 365
- Productivity
- Tasks
---
