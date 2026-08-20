---
api_key_in: []
api_specs:
- filename: cometapi-audio-api-openapi.yml
  format: yaml
  label: CometAPI Audio API
  slug: cometapi-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-audio-api-openapi.yml
- filename: cometapi-chat-api-openapi.yml
  format: yaml
  label: CometAPI Chat API
  slug: cometapi-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-chat-api-openapi.yml
- filename: cometapi-embeddings-api-openapi.yml
  format: yaml
  label: CometAPI Embeddings API
  slug: cometapi-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-embeddings-api-openapi.yml
- filename: cometapi-images-api-openapi.yml
  format: yaml
  label: CometAPI Images API
  slug: cometapi-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-images-api-openapi.yml
- filename: cometapi-models-api-openapi.yml
  format: yaml
  label: CometAPI Models API
  slug: cometapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-models-api-openapi.yml
- filename: cometapi-video-api-openapi.yml
  format: yaml
  label: CometAPI Video API
  slug: cometapi-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-video-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cometapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: CometAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CometAPI
provider_slug: cometapi
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cometapi-unified-api-openapi.yml
  type: http
slug: cometapi-authentication
source_filename: cometapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cometapi-unified-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cometapi-unified-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/authentication/cometapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Aggregator
- Audio
- Chat
- Embeddings
- Generative AI
- Image
- LLM
- Multi-Model
- OpenAI-Compatible
- Video
---
