---
api_key_in: []
api_specs:
- filename: 01-ai-openapi.yml
  format: yaml
  label: Lingyiwanwu Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/01-ai/refs/heads/main/openapi/01-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 01 Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: 01.AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 01.AI
provider_slug: 01-ai
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/01-ai-openapi.yml
  type: http
slug: 01-ai-authentication
source_filename: 01-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/01-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/01-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/01-ai/refs/heads/main/authentication/01-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Yi
- Open Source
- Foundation Models
- Inference
---
