---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cometapi-models-api-openapi.yml
  format: yaml
  label: CometAPI Models API
  slug: cometapi-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cometapi/openapi/cometapi-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CometAPI Authentication
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
source_yaml_url: https://artifacts.apis.io/cometapi/authentication/cometapi-authentication.yml
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
