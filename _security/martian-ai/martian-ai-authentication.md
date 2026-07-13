---
api_key_in: []
api_specs:
- filename: martian-ai-openapi.yml
  format: yaml
  label: Martian Chat Completions API
  slug: martian-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/martian-ai/refs/heads/main/openapi/martian-ai-openapi.yml
- filename: martian-ai-openapi.yml
  format: yaml
  label: Martian Messages API
  slug: martian-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/martian-ai/refs/heads/main/openapi/martian-ai-openapi.yml
- filename: martian-ai-openapi.yml
  format: yaml
  label: Martian Models API
  slug: martian-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/martian-ai/refs/heads/main/openapi/martian-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Martian Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Martian secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Martian
provider_slug: martian-ai
scheme_count: 1
schemes:
- description: Provide your Martian API key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/martian-ai-openapi.yml
  type: http
slug: martian-ai-authentication
source_filename: martian-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/martian-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Provide your Martian API key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/martian-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/martian-ai/refs/heads/main/authentication/martian-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Model Router
- Gateway
- Cost Optimization
---
