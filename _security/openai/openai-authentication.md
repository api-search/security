---
api_key_in: []
api_specs:
- filename: assistants-openapi-original.yml
  format: yaml
  label: OpenAI Assistants API
  slug: openai-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/assistants-openapi-original.yml
- filename: audio-openapi-original.yml
  format: yaml
  label: OpenAI Audio API
  slug: openai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/audio-openapi-original.yml
- filename: chat-openapi-original.yml
  format: yaml
  label: OpenAI Chat API
  slug: openai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/chat-openapi-original.yml
- filename: openai-chat-completions-api-openapi.yml
  format: yaml
  label: OpenAI Chat Completions API
  slug: openai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/properties/openai-chat-completions-api-openapi.yml
- filename: embeddings-openapi-original.yml
  format: yaml
  label: OpenAI Embeddings API
  slug: openai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/embeddings-openapi-original.yml
- filename: files-openapi-original.yml
  format: yaml
  label: OpenAI Files API
  slug: openai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/files-openapi-original.yml
- filename: fine-tuning-openapi-original.yml
  format: yaml
  label: OpenAI Fine Tuning API
  slug: openai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/fine-tuning-openapi-original.yml
- filename: images-openapi-original.yml
  format: yaml
  label: OpenAI Images API
  slug: openai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/images-openapi-original.yml
- filename: models-openapi-original.yml
  format: yaml
  label: OpenAI Models API
  slug: openai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/models-openapi-original.yml
- filename: threads-openapi-original.yml
  format: yaml
  label: OpenAI Threads API
  slug: openai-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/threads-openapi-original.yml
- filename: openai-realtime-asyncapi.yml
  format: yaml
  label: OpenAI Realtime API
  slug: openai-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/asyncapi/openai-realtime-asyncapi.yml
- filename: completions-openapi-original.yml
  format: yaml
  label: OpenAI Completions API
  slug: openai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/completions-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openai Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenAI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenAI
provider_slug: openai
scheme_count: 1
schemes:
- name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/assistants-openapi-original.yml
  - openapi/audio-openapi-original.yml
  - openapi/chat-openapi-original.yml
  - openapi/completions-openapi-original.yml
  - openapi/embeddings-openapi-original.yml
  - openapi/files-openapi-original.yml
  - openapi/fine-tuning-openapi-original.yml
  - openapi/images-openapi-original.yml
  - openapi/models-openapi-original.yml
  - openapi/openai-audio-openapi.yml
  - openapi/openai-chat-completions-openapi.yml
  - openapi/openai-embeddings-openapi.yml
  - openapi/openai-images-openapi.yml
  - openapi/openai-openapi-master.yml
  - openapi/threads-openapi-original.yml
  type: http
slug: openai-authentication
source_filename: openai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/assistants-openapi-original.yml, openapi/audio-openapi-original.yml, openapi/chat-openapi-original.yml,\n  openapi/completions-openapi-original.yml, openapi/embeddings-openapi-original.yml, openapi/files-openapi-original.yml,\n  openapi/fine-tuning-openapi-original.yml, openapi/images-openapi-original.yml, openapi/models-openapi-original.yml,\n  openapi/openai-audio-openapi.yml, openapi/openai-chat-completions-openapi.yml, openapi/openai-embeddings-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/assistants-openapi-original.yml\n  - openapi/audio-openapi-original.yml\n  - openapi/chat-openapi-original.yml\n  - openapi/completions-openapi-original.yml\n  - openapi/embeddings-openapi-original.yml\n  - openapi/files-openapi-original.yml\n  - openapi/fine-tuning-openapi-original.yml\n  - openapi/images-openapi-original.yml\n  - openapi/models-openapi-original.yml\n\
  \  - openapi/openai-audio-openapi.yml\n  - openapi/openai-chat-completions-openapi.yml\n  - openapi/openai-embeddings-openapi.yml\n  - openapi/openai-images-openapi.yml\n  - openapi/openai-openapi-master.yml\n  - openapi/threads-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/authentication/openai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
---
