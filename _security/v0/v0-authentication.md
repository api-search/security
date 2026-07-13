---
api_key_in:
- header
api_specs:
- filename: v0-platform-openapi.json
  format: json
  label: v0 Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v0/refs/heads/main/openapi/v0-platform-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: V0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: v0 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: v0
provider_slug: v0
scheme_count: 1
schemes:
- description: Your v0 API key. Get one at https://v0.app/chat/settings/keys
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/v0-platform-openapi.json
  type: apiKey
slug: v0-authentication
source_filename: v0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/v0-platform-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Your v0 API key. Get one at https://v0.app/chat/settings/keys\n  sources:\n  - openapi/v0-platform-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/v0/refs/heads/main/authentication/v0-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- App Builder
- Vercel
- Code Generation
- Platform API
---
