---
api_key_in: []
api_specs:
- filename: openai-chat-completions-openapi.yml
  format: yaml
  label: OpenAI Chat Completions API
  slug: openai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-chat-completions-openapi.yml
- filename: openai-completions-openapi.yml
  format: yaml
  label: OpenAI Completions API
  slug: openai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-completions-openapi.yml
- filename: openai-images-openapi.yml
  format: yaml
  label: OpenAI Images API
  slug: openai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-images-openapi.yml
- filename: openai-embeddings-openapi.yml
  format: yaml
  label: OpenAI Embeddings API
  slug: openai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-embeddings-openapi.yml
- filename: openai-audio-openapi.yml
  format: yaml
  label: OpenAI Audio API
  slug: openai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-audio-openapi.yml
- filename: openai-moderations-openapi.yml
  format: yaml
  label: OpenAI Moderations API
  slug: openai-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-moderations-openapi.yml
- filename: openai-assistants-openapi.yml
  format: yaml
  label: OpenAI Assistants API
  slug: openai-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-assistants-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openai Apis Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenAI APIs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenAI APIs
provider_slug: openai-apis
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: OpenAI API key passed as a Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openai-assistants-openapi.yml
  - openapi/openai-audio-openapi.yml
  - openapi/openai-chat-completions-openapi.yml
  - openapi/openai-completions-openapi.yml
  - openapi/openai-embeddings-openapi.yml
  - openapi/openai-images-openapi.yml
  - openapi/openai-moderations-openapi.yml
  type: http
slug: openai-apis-authentication
source_filename: openai-apis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openai-assistants-openapi.yml, openapi/openai-audio-openapi.yml, openapi/openai-chat-completions-openapi.yml,\n  openapi/openai-completions-openapi.yml, openapi/openai-embeddings-openapi.yml, openapi/openai-images-openapi.yml,\n  openapi/openai-moderations-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: OpenAI API key passed as a Bearer token\n  sources:\n  - openapi/openai-assistants-openapi.yml\n  - openapi/openai-audio-openapi.yml\n  - openapi/openai-chat-completions-openapi.yml\n  - openapi/openai-completions-openapi.yml\n  - openapi/openai-embeddings-openapi.yml\n  - openapi/openai-images-openapi.yml\n  - openapi/openai-moderations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/authentication/openai-apis-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Embeddings
- Image Generation
- Language Models
- Speech
---
