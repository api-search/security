---
api_key_in: []
api_specs:
- filename: granola-openapi.yml
  format: yaml
  label: Granola Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/granola/refs/heads/main/openapi/granola-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Granola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Granola secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Granola
provider_slug: granola
scheme_count: 1
schemes:
- bearerFormat: API key (grn_...)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/granola-openapi.yml
  type: http
slug: granola-authentication
source_filename: granola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/granola-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key (grn_...)\n  sources:\n  - openapi/granola-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granola/refs/heads/main/authentication/granola-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Meeting Notes
- Transcription
- Productivity
- API
- MCP
- Zapier
- Business
- Enterprise
---
