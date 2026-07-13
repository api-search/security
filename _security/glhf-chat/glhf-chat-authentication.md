---
api_key_in: []
api_specs:
- filename: glhf-chat-openapi.yml
  format: yaml
  label: glhf Chat Completions API
  slug: glhf-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glhf-chat/refs/heads/main/openapi/glhf-chat-openapi.yml
- filename: glhf-chat-openapi.yml
  format: yaml
  label: glhf Models API
  slug: glhf-chat-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glhf-chat/refs/heads/main/openapi/glhf-chat-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Glhf Chat Authentication
name_suffix: Authentication
oauth_flows: []
overview: glhf secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: glhf
provider_slug: glhf-chat
scheme_count: 1
schemes:
- description: glhf API key passed as a Bearer token in the Authorization header. Keys are created at https://glhf.chat/users/settings/api.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/glhf-chat-openapi.yml
  type: http
slug: glhf-chat-authentication
source_filename: glhf-chat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glhf-chat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: glhf API key passed as a Bearer token in the Authorization header. Keys are created\n    at https://glhf.chat/users/settings/api.\n  sources:\n  - openapi/glhf-chat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glhf-chat/refs/heads/main/authentication/glhf-chat-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Open Source Models
- Hugging Face
---
