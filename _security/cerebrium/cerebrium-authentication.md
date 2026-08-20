---
api_key_in: []
api_specs:
- filename: cerebrium-inference-api-openapi.yml
  format: yaml
  label: Cerebrium Inference API
  slug: cerebrium-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/openapi/cerebrium-inference-api-openapi.yml
- filename: cerebrium-openai-compatible-api-openapi.yml
  format: yaml
  label: Cerebrium OpenAI Compatible API
  slug: cerebrium-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/openapi/cerebrium-openai-compatible-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cerebrium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cerebrium secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cerebrium
provider_slug: cerebrium
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT token from the dashboard API Keys section, sent as Authorization: Bearer <JWT_TOKEN>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cerebrium-openapi.yml
  type: http
slug: cerebrium-authentication
source_filename: cerebrium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cerebrium-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT token from the dashboard API Keys section, sent as Authorization: Bearer\n    <JWT_TOKEN>.'\n  sources:\n  - openapi/cerebrium-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/authentication/cerebrium-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- GPU
- Serverless
- Inference
- ML Infrastructure
---
