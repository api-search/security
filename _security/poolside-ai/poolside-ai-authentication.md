---
api_key_in: []
api_specs:
- filename: poolside-ai-openapi.json
  format: json
  label: Poolside Chat Completions API
  slug: poolside-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/openapi/poolside-ai-openapi.json
- filename: poolside-ai-openapi.json
  format: json
  label: Poolside Completions API (Legacy)
  slug: poolside-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/openapi/poolside-ai-openapi.json
- filename: poolside-ai-openapi.json
  format: json
  label: Poolside Models API
  slug: poolside-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/openapi/poolside-ai-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Poolside Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Poolside secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Poolside
provider_slug: poolside-ai
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/poolside-ai-openapi.json
  type: http
slug: poolside-ai-authentication
source_filename: poolside-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/poolside-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/poolside-ai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/authentication/poolside-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Foundation Models
- Agentic Coding
- Software Engineering
- Enterprise
- On-Prem
- Open Weights
---
