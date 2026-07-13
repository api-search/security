---
api_key_in: []
api_specs:
- filename: deepseek-chat-completion-api-openapi.yml
  format: yaml
  label: DeepSeek Chat Completion API
  slug: deepseek-chat-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-chat-completion-api-openapi.yml
- filename: deepseek-fim-completion-openapi.yml
  format: yaml
  label: DeepSeek Fill-In-The-Middle (FIM) Completion API
  slug: deepseek-fim-completion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-fim-completion-openapi.yml
- filename: deepseek-lists-models-api-openapi.yml
  format: yaml
  label: DeepSeek List Models API
  slug: deepseek-lists-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-lists-models-api-openapi.yml
- filename: deepseek-user-balance-api-openapi.yml
  format: yaml
  label: DeepSeek User Balance API
  slug: deepseek-user-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/openapi/deepseek-user-balance-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deepseek Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepSeek secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeepSeek
provider_slug: deepseek
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deepseek-lists-models-api-openapi.yml
  - openapi/deepseek-user-balance-api-openapi.yml
  type: http
slug: deepseek-authentication
source_filename: deepseek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepseek-lists-models-api-openapi.yml, openapi/deepseek-user-balance-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/deepseek-lists-models-api-openapi.yml\n  - openapi/deepseek-user-balance-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepseek/refs/heads/main/authentication/deepseek-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Chat
- Chat Completion
- LLM
- Large Language Models
- Reasoning
- Code Completion
---
