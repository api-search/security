---
api_key_in: []
api_specs:
- filename: hyperbolic-chat-completions-api-openapi.yml
  format: yaml
  label: Hyperbolic Chat Completions API
  slug: hyperbolic-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-chat-completions-api-openapi.yml
- filename: hyperbolic-completions-api-openapi.yml
  format: yaml
  label: Hyperbolic Completions API
  slug: hyperbolic-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-completions-api-openapi.yml
- filename: hyperbolic-image-generation-api-openapi.yml
  format: yaml
  label: Hyperbolic Image Generation API
  slug: hyperbolic-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-image-generation-api-openapi.yml
- filename: hyperbolic-audio-generation-api-openapi.yml
  format: yaml
  label: Hyperbolic Audio Generation API
  slug: hyperbolic-audio-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-audio-generation-api-openapi.yml
- filename: hyperbolic-models-api-openapi.yml
  format: yaml
  label: Hyperbolic Models API
  slug: hyperbolic-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hyperbolic Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperbolic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hyperbolic
provider_slug: hyperbolic-ai
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hyperbolic-audio-generation-api-openapi.yml
  - openapi/hyperbolic-chat-completions-api-openapi.yml
  - openapi/hyperbolic-completions-api-openapi.yml
  - openapi/hyperbolic-image-generation-api-openapi.yml
  - openapi/hyperbolic-models-api-openapi.yml
  type: http
slug: hyperbolic-ai-authentication
source_filename: hyperbolic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperbolic-audio-generation-api-openapi.yml, openapi/hyperbolic-chat-completions-api-openapi.yml,\n  openapi/hyperbolic-completions-api-openapi.yml, openapi/hyperbolic-image-generation-api-openapi.yml,\n  openapi/hyperbolic-models-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/hyperbolic-audio-generation-api-openapi.yml\n  - openapi/hyperbolic-chat-completions-api-openapi.yml\n  - openapi/hyperbolic-completions-api-openapi.yml\n  - openapi/hyperbolic-image-generation-api-openapi.yml\n  - openapi/hyperbolic-models-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/authentication/hyperbolic-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Compute
- Decentralized
- DePIN
- GPU
- Image Generation
- Inference
- LLM
- Marketplace
- Open Source
---
