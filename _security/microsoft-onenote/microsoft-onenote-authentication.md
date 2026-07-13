---
api_key_in: []
api_specs:
- filename: microsoft-onenote-openapi.yml
  format: yaml
  label: Microsoft Graph OneNote API
  slug: graph-onenote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/openapi/microsoft-onenote-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Onenote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft OneNote secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft OneNote
provider_slug: microsoft-onenote
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-onenote-openapi.yml
  type: http
slug: microsoft-onenote-authentication
source_filename: microsoft-onenote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-onenote-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-onenote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/authentication/microsoft-onenote-authentication.yml
summary_line: http · 1 scheme
tags:
- Microsoft
- Microsoft 365
- Notebooks
- Notes
- Productivity
---
