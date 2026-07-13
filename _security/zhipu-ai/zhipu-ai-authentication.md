---
api_key_in: []
api_specs:
- filename: zhipu-ai-openapi.json
  format: json
  label: Z.ai Open Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zhipu-ai/refs/heads/main/openapi/zhipu-ai-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zhipu Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zhipu AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zhipu AI
provider_slug: zhipu-ai
scheme_count: 1
schemes:
- description: 'Use the following format for authentication: Bearer [<your api key>](https://z.ai/manage-apikey/apikey-list)'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zhipu-ai-openapi.json
  type: http
slug: zhipu-ai-authentication
source_filename: zhipu-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zhipu-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Use the following format for authentication: Bearer [<your api key>](https://z.ai/manage-apikey/apikey-list)'\n  sources:\n  - openapi/zhipu-ai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhipu-ai/refs/heads/main/authentication/zhipu-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- GLM
- ChatGLM
- Multimodal
---
