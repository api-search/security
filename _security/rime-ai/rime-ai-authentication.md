---
api_key_in: []
api_specs:
- filename: rime-ai-plants-api-openapi.yml
  format: yaml
  label: Rime Plants API
  slug: rime-ai-plants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rime-ai/refs/heads/main/openapi/rime-ai-plants-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rime Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rime secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rime
provider_slug: rime-ai
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rime-ai-openapi.json
  type: http
slug: rime-ai-authentication
source_filename: rime-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rime-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/rime-ai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rime-ai/refs/heads/main/authentication/rime-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Voice
- TTS
- Real-Time
- Conversational
---
