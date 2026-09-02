---
api_key_in: []
api_specs:
- filename: doubao-batch-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Batch API
  slug: doubao-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-batch-api-openapi.yml
- filename: doubao-chat-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Chat API
  slug: doubao-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-chat-api-openapi.yml
- filename: doubao-embeddings-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Embeddings API
  slug: doubao-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-embeddings-api-openapi.yml
- filename: doubao-images-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Images API
  slug: doubao-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-images-api-openapi.yml
- filename: doubao-videos-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Videos API
  slug: doubao-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Doubao Authentication
name_suffix: Authentication
oauth_flows: []
overview: ByteDance Doubao secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ByteDance Doubao
provider_slug: doubao
scheme_count: 1
schemes:
- bearerFormat: Ark API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/doubao-openapi.yml
  type: http
slug: doubao-authentication
source_filename: doubao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/doubao-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Ark API Key\n  sources:\n  - openapi/doubao-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/authentication/doubao-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Inference
- ByteDance
- Multi-Modal
- Volcano Engine
---
