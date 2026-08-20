---
api_key_in: []
api_specs:
- filename: aimlapi-api-key-management-api-openapi.yml
  format: yaml
  label: AIMLAPI API Key Management API
  slug: aimlapi-api-key-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-api-key-management-api-openapi.yml
- filename: aimlapi-assistants-api-openapi.yml
  format: yaml
  label: AIMLAPI Assistants API
  slug: aimlapi-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-assistants-api-openapi.yml
- filename: aimlapi-chat-api-openapi.yml
  format: yaml
  label: AIMLAPI Chat API
  slug: aimlapi-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-chat-api-openapi.yml
- filename: aimlapi-images-api-openapi.yml
  format: yaml
  label: AIMLAPI Images API
  slug: aimlapi-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-images-api-openapi.yml
- filename: aimlapi-models-api-openapi.yml
  format: yaml
  label: AIMLAPI Models API
  slug: aimlapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-models-api-openapi.yml
- filename: aimlapi-threads-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads API
  slug: aimlapi-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-api-openapi.yml
- filename: aimlapi-threads-messages-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads > Messages API
  slug: aimlapi-threads-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-messages-api-openapi.yml
- filename: aimlapi-threads-runs-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads > Runs API
  slug: aimlapi-threads-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-runs-api-openapi.yml
- filename: aimlapi-voice-api-openapi.yml
  format: yaml
  label: AIMLAPI Voice API
  slug: aimlapi-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-voice-api-openapi.yml
- filename: aimlapi-wip-completions-api-openapi.yml
  format: yaml
  label: AIMLAPI [WIP] Completions API
  slug: aimlapi-wip-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-wip-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aimlapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIMLAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AIMLAPI
provider_slug: aimlapi
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aimlapi-openapi.yml
  type: http
slug: aimlapi-authentication
source_filename: aimlapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aimlapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/aimlapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/authentication/aimlapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Machine-Learning
- AI Models
- LLM
- Image-Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
---
