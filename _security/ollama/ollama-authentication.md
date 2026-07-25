---
api_key_in: []
api_specs:
- filename: ollama-blobs-api-openapi.yml
  format: yaml
  label: Ollama Blobs API
  slug: ollama-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-blobs-api-openapi.yml
- filename: ollama-chat-api-openapi.yml
  format: yaml
  label: Ollama Chat API
  slug: ollama-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-chat-api-openapi.yml
- filename: ollama-chat-completions-api-openapi.yml
  format: yaml
  label: Ollama Chat Completions API
  slug: ollama-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-chat-completions-api-openapi.yml
- filename: ollama-completions-api-openapi.yml
  format: yaml
  label: Ollama Completions API
  slug: ollama-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-completions-api-openapi.yml
- filename: ollama-embeddings-api-openapi.yml
  format: yaml
  label: Ollama Embeddings API
  slug: ollama-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-embeddings-api-openapi.yml
- filename: ollama-generate-api-openapi.yml
  format: yaml
  label: Ollama Generate API
  slug: ollama-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-generate-api-openapi.yml
- filename: ollama-images-api-openapi.yml
  format: yaml
  label: Ollama Images API
  slug: ollama-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-images-api-openapi.yml
- filename: ollama-models-api-openapi.yml
  format: yaml
  label: Ollama Models API
  slug: ollama-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-models-api-openapi.yml
- filename: ollama-responses-api-openapi.yml
  format: yaml
  label: Ollama Responses API
  slug: ollama-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-responses-api-openapi.yml
- filename: ollama-running-models-api-openapi.yml
  format: yaml
  label: Ollama Running Models API
  slug: ollama-running-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-running-models-api-openapi.yml
- filename: ollama-version-api-openapi.yml
  format: yaml
  label: Ollama Version API
  slug: ollama-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-version-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ollama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ollama secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ollama
provider_slug: ollama
scheme_count: 1
schemes:
- description: API key authentication. The key is accepted but not validated by Ollama. Use any value such as ollama.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ollama-openai-compatibility-api-openapi.yml
  type: http
slug: ollama-authentication
source_filename: ollama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ollama-openai-compatibility-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication. The key is accepted but not validated by Ollama. Use\n    any value such as ollama.\n  sources:\n  - openapi/ollama-openai-compatibility-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/authentication/ollama-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Large Language Models
- Models
---
