---
api_key_in: []
api_specs:
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Chat Completions API
  slug: fireworks-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Completions API
  slug: fireworks-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Vision API
  slug: fireworks-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Embeddings API
  slug: fireworks-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Rerank API
  slug: fireworks-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Images API
  slug: fireworks-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Audio API
  slug: fireworks-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Batch Inference API
  slug: fireworks-batch-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Fine-Tuning API
  slug: fireworks-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Files API
  slug: fireworks-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Models API
  slug: fireworks-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Deployments API
  slug: fireworks-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Account API
  slug: fireworks-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fireworks Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fireworks AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fireworks AI
provider_slug: fireworks-ai
scheme_count: 1
schemes:
- bearerFormat: API_KEY
  description: 'Bearer authentication using your Fireworks API key. Format: Bearer <API_KEY>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fireworks-ai-anthropic-messages-openapi.json
  - openapi/fireworks-ai-gateway-openapi.yml
  - openapi/fireworks-ai-merged-openapi.yml
  - openapi/fireworks-ai-responses-openapi.yml
  - openapi/fireworks-ai-text-completion-openapi.yml
  type: http
slug: fireworks-ai-authentication
source_filename: fireworks-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fireworks-ai-anthropic-messages-openapi.json, openapi/fireworks-ai-gateway-openapi.yml,\n  openapi/fireworks-ai-merged-openapi.yml, openapi/fireworks-ai-responses-openapi.yml, openapi/fireworks-ai-text-completion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API_KEY\n  description: 'Bearer authentication using your Fireworks API key. Format: Bearer <API_KEY>'\n  sources:\n  - openapi/fireworks-ai-anthropic-messages-openapi.json\n  - openapi/fireworks-ai-gateway-openapi.yml\n  - openapi/fireworks-ai-merged-openapi.yml\n  - openapi/fireworks-ai-responses-openapi.yml\n  - openapi/fireworks-ai-text-completion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/authentication/fireworks-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Multimodal
- Fine-tuning
- GPU
---
