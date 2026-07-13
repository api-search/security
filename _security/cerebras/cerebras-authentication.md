---
api_key_in: []
api_specs:
- filename: cerebras-openapi.yml
  format: yaml
  label: Cerebras Inference API
  slug: cerebras-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebras/refs/heads/main/openapi/cerebras-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cerebras Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cerebras secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cerebras
provider_slug: cerebras
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Provision a CEREBRAS_API_KEY at https://cloud.cerebras.ai
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cerebras-openapi.yml
  type: http
slug: cerebras-authentication
source_filename: cerebras-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cerebras-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Provision a CEREBRAS_API_KEY at https://cloud.cerebras.ai\n  sources:\n  - openapi/cerebras-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebras/refs/heads/main/authentication/cerebras-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Inference
- Large Language Models
- Wafer Scale
- Hardware
- Cloud
- OpenAI Compatible
- LLM
- SDK
- Accelerator
- High Performance Computing
---
