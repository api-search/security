---
api_key_in: []
api_specs:
- filename: eden-ai-openapi.yml
  format: yaml
  label: Eden AI API
  slug: eden-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/eden-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Eden Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eden AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eden AI
provider_slug: eden-ai
scheme_count: 1
schemes:
- bearerFormat: API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eden-ai-openapi.yml
  type: http
slug: eden-ai-authentication
source_filename: eden-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eden-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/eden-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/authentication/eden-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Emotion
- Emotion Detection
---
