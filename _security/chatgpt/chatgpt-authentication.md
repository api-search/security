---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: ChatGPT API
  slug: chatgpt-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Responses API
  slug: openai-responses-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chatgpt Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChatGPT secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ChatGPT
provider_slug: chatgpt
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'API key authentication using Bearer token. Pass your OpenAI API

    key as a Bearer token in the Authorization header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/chatgpt-chat-completions-api-openapi.yml
  - openapi/chatgpt-responses-api-openapi.yml
  type: http
slug: chatgpt-authentication
source_filename: chatgpt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chatgpt-chat-completions-api-openapi.yml, openapi/chatgpt-responses-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    API key authentication using Bearer token. Pass your OpenAI API\n    key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/chatgpt-chat-completions-api-openapi.yml\n  - openapi/chatgpt-responses-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/authentication/chatgpt-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- Artificial Intelligence
- ChatGPT
- Embeddings
- Fine-Tuning
- GPT-4
- GPT-5
- Language Model
- OpenAI
- Real-Time
---
