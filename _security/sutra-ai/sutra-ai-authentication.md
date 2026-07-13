---
api_key_in: []
api_specs:
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Chat Completions (Multilingual) API
  slug: chat-completions-multilingual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Reasoning API
  slug: reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sutra Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: SUTRA (Two AI) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SUTRA (Two AI)
provider_slug: sutra-ai
scheme_count: 1
schemes:
- description: 'Provide your SUTRA API key as a Bearer token in the Authorization header - Authorization: Bearer <YOUR_SUTRA_API_KEY>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sutra-ai-openapi.yml
  type: http
slug: sutra-ai-authentication
source_filename: sutra-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sutra-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Provide your SUTRA API key as a Bearer token in the Authorization header - Authorization:\n    Bearer <YOUR_SUTRA_API_KEY>.'\n  sources:\n  - openapi/sutra-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/authentication/sutra-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Multilingual
- Inference
- Reasoning
---
