---
api_key_in: []
api_specs:
- filename: openai-apis-assistants-api-openapi.yml
  format: yaml
  label: OpenAI APIs Assistants API
  slug: openai-apis-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-assistants-api-openapi.yml
- filename: openai-apis-chat-api-openapi.yml
  format: yaml
  label: OpenAI APIs Chat API
  slug: openai-apis-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-chat-api-openapi.yml
- filename: openai-apis-completions-api-openapi.yml
  format: yaml
  label: OpenAI APIs Completions API
  slug: openai-apis-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-completions-api-openapi.yml
- filename: openai-apis-embeddings-api-openapi.yml
  format: yaml
  label: OpenAI APIs Embeddings API
  slug: openai-apis-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-embeddings-api-openapi.yml
- filename: openai-apis-images-api-openapi.yml
  format: yaml
  label: OpenAI APIs Images API
  slug: openai-apis-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-images-api-openapi.yml
- filename: openai-apis-messages-api-openapi.yml
  format: yaml
  label: OpenAI APIs Messages API
  slug: openai-apis-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-messages-api-openapi.yml
- filename: openai-apis-moderations-api-openapi.yml
  format: yaml
  label: OpenAI APIs Moderations API
  slug: openai-apis-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-moderations-api-openapi.yml
- filename: openai-apis-runs-api-openapi.yml
  format: yaml
  label: OpenAI APIs Runs API
  slug: openai-apis-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-runs-api-openapi.yml
- filename: openai-apis-speech-api-openapi.yml
  format: yaml
  label: OpenAI APIs Speech API
  slug: openai-apis-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-speech-api-openapi.yml
- filename: openai-apis-threads-api-openapi.yml
  format: yaml
  label: OpenAI APIs Threads API
  slug: openai-apis-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-threads-api-openapi.yml
- filename: openai-apis-transcription-api-openapi.yml
  format: yaml
  label: OpenAI APIs Transcription API
  slug: openai-apis-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-transcription-api-openapi.yml
- filename: openai-apis-translation-api-openapi.yml
  format: yaml
  label: OpenAI APIs Translation API
  slug: openai-apis-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-translation-api-openapi.yml
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
