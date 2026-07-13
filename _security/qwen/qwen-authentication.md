---
api_key_in: []
api_specs:
- filename: qwen-openapi.yml
  format: yaml
  label: DashScope (Alibaba Cloud Model Studio) API
  slug: dashscope
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwen/refs/heads/main/openapi/qwen-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qwen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qwen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qwen
provider_slug: qwen
scheme_count: 1
schemes:
- description: 'Bearer API key from the DashScope key management page. Pass as `Authorization: Bearer <DASHSCOPE_API_KEY>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/qwen-openapi.yml
  type: http
slug: qwen-authentication
source_filename: qwen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qwen-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key from the DashScope key management page. Pass as `Authorization:\n    Bearer <DASHSCOPE_API_KEY>`.'\n  sources:\n  - openapi/qwen-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwen/refs/heads/main/authentication/qwen-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Open Source
- Alibaba
- Multimodal
---
