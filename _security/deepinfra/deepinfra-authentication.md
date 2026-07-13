---
api_key_in: []
api_specs:
- filename: deepinfra-openapi.yml
  format: yaml
  label: DeepInfra Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepinfra/refs/heads/main/openapi/deepinfra-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deepinfra Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepInfra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeepInfra
provider_slug: deepinfra
scheme_count: 1
schemes:
- description: DeepInfra API token (DEEPINFRA_TOKEN) sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deepinfra-openapi.yml
  type: http
slug: deepinfra-authentication
source_filename: deepinfra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepinfra-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: DeepInfra API token (DEEPINFRA_TOKEN) sent as a Bearer token.\n  sources:\n  - openapi/deepinfra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepinfra/refs/heads/main/authentication/deepinfra-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Serverless
- Open Source
- OpenAI Compatible
- Anthropic Compatible
- Image Generation
- Audio
- Embeddings
---
