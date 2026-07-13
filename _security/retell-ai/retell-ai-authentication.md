---
api_key_in: []
api_specs:
- filename: retell-ai-openapi.yml
  format: yaml
  label: Retell AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell-ai/refs/heads/main/openapi/retell-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Retell Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Retell AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Retell AI
provider_slug: retell-ai
scheme_count: 1
schemes:
- bearerFormat: string
  description: Authentication header containing API key (find it in dashboard). The format is "Bearer YOUR_API_KEY"
  name: api_key
  scheme: bearer
  sources:
  - openapi/retell-ai-openapi.yml
  type: http
slug: retell-ai-authentication
source_filename: retell-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/retell-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: string\n  description: Authentication header containing API key (find it in dashboard). The format is\n    \"Bearer YOUR_API_KEY\"\n  sources:\n  - openapi/retell-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retell-ai/refs/heads/main/authentication/retell-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice
- Agents
- Realtime
- Conversational
---
