---
api_key_in: []
api_specs:
- filename: cometapi-unified-api-openapi.yml
  format: yaml
  label: CometAPI Unified API
  slug: cometapi-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-unified-api-openapi.yml
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
- AI
- Aggregator
- Audio
- Chat
- Embeddings
- Generative AI
- Images
- LLM
- Multi-Model
- OpenAI-Compatible
- Video
---
