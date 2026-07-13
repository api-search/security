---
api_key_in: []
api_specs:
- filename: vapi-openapi.yml
  format: yaml
  label: Vapi Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi/refs/heads/main/openapi/vapi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vapi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vapi
provider_slug: vapi
scheme_count: 1
schemes:
- bearerFormat: Bearer
  description: Retrieve your API Key from [Dashboard](dashboard.vapi.ai).
  name: bearer
  scheme: bearer
  sources:
  - openapi/vapi-openapi.yml
  type: http
slug: vapi-authentication
source_filename: vapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer\n  description: Retrieve your API Key from [Dashboard](dashboard.vapi.ai).\n  sources:\n  - openapi/vapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vapi/refs/heads/main/authentication/vapi-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice
- Agents
- Realtime
- CPaaS
---
