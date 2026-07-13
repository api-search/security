---
api_key_in: []
api_specs:
- filename: vllm-openapi.yml
  format: yaml
  label: vLLM OpenAI-Compatible Server
  slug: openai-compatible
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vllm/refs/heads/main/openapi/vllm-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vllm Authentication
name_suffix: Authentication
oauth_flows: []
overview: vLLM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: vLLM
provider_slug: vllm
scheme_count: 1
schemes:
- description: API key supplied at server startup via --api-key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vllm-openapi.yml
  type: http
slug: vllm-authentication
source_filename: vllm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vllm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key supplied at server startup via --api-key\n  sources:\n  - openapi/vllm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vllm/refs/heads/main/authentication/vllm-authentication.yml
summary_line: http · 1 scheme
tags:
- LLM
- Inference
- Open Source
- GPU
- OpenAI Compatible
- Self-Hosted
---
