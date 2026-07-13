---
api_key_in: []
api_specs:
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI LLM Proxy (Chat Completions)
  slug: llm-proxy-chat-completions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Logging API
  slug: logging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Prompts API
  slug: prompts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Threads API
  slug: threads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Evaluations API
  slug: evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Traces API
  slug: traces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Keywordsai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keywords AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Keywords AI
provider_slug: keywordsai
scheme_count: 1
schemes:
- description: 'Keywords AI API key supplied as the Authorization Bearer header (Authorization: Bearer <KEYWORDSAI_API_KEY>).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keywordsai-openapi.yml
  type: http
slug: keywordsai-authentication
source_filename: keywordsai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keywordsai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Keywords AI API key supplied as the Authorization Bearer header (Authorization:\n    Bearer <KEYWORDSAI_API_KEY>).'\n  sources:\n  - openapi/keywordsai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/authentication/keywordsai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Observability
- Gateway
- Monitoring
---
