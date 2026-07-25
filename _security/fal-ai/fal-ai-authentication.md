---
api_key_in:
- header
api_specs:
- filename: fal-ai-asyncapi.yml
  format: yaml
  label: fal Realtime API
  slug: fal-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/asyncapi/fal-ai-asyncapi.yml
- filename: fal-ai-asyncapi.yml
  format: yaml
  label: fal Streaming API
  slug: fal-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/asyncapi/fal-ai-asyncapi.yml
- filename: fal-ai-apps-api-openapi.yml
  format: yaml
  label: fal Apps API
  slug: fal-ai-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-ai-apps-api-openapi.yml
- filename: fal-ai-files-api-openapi.yml
  format: yaml
  label: fal Files API
  slug: fal-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-ai-files-api-openapi.yml
- filename: fal-ai-queue-api-openapi.yml
  format: yaml
  label: fal Queue API
  slug: fal-ai-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-ai-queue-api-openapi.yml
- filename: fal-ai-secrets-api-openapi.yml
  format: yaml
  label: fal Secrets API
  slug: fal-ai-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-ai-secrets-api-openapi.yml
- filename: fal-ai-storage-api-openapi.yml
  format: yaml
  label: fal Storage API
  slug: fal-ai-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-ai-storage-api-openapi.yml
- filename: fal-ai-streaming-api-openapi.yml
  format: yaml
  label: fal Streaming API
  slug: fal-ai-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-ai-streaming-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fal Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: fal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: fal
provider_slug: fal-ai
scheme_count: 1
schemes:
- description: 'Pass the fal API key as `Authorization: Key $FAL_KEY`. Keys are issued from the fal dashboard at https://fal.ai/dashboard/keys.'
  in: header
  name: FalKeyAuth
  parameter: Authorization
  sources:
  - openapi/fal-model-apis-openapi.yml
  - openapi/fal-serverless-platform-api-openapi.yml
  - openapi/fal-storage-api-openapi.yml
  type: apiKey
slug: fal-ai-authentication
source_filename: fal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fal-model-apis-openapi.yml, openapi/fal-serverless-platform-api-openapi.yml,\n  openapi/fal-storage-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: FalKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Pass the fal API key as `Authorization: Key $FAL_KEY`. Keys are issued from\n    the fal dashboard at https://fal.ai/dashboard/keys.'\n  sources:\n  - openapi/fal-model-apis-openapi.yml\n  - openapi/fal-serverless-platform-api-openapi.yml\n  - openapi/fal-storage-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/authentication/fal-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Artificial Intelligence
- Generative AI
- Generative Media
- Image Generation
- Video Generation
- Audio Generation
- Inference
- Serverless
- GPU
- MCP
---
