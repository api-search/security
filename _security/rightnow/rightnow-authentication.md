---
api_key_in: []
api_specs:
- filename: rightnow-openapi.json
  format: json
  label: RunInfra Inference API
  slug: runinfra-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rightnow Authentication
name_suffix: Authentication
oauth_flows: []
overview: RightNow AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RightNow AI
provider_slug: rightnow
scheme_count: 1
schemes:
- description: RunInfra API key. Generate at https://runinfra.ai/settings/api-keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rightnow-openapi.json
  type: http
slug: rightnow-authentication
source_filename: rightnow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rightnow-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: RunInfra API key. Generate at https://runinfra.ai/settings/api-keys\n  sources:\n  - openapi/rightnow-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/authentication/rightnow-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM Inference
- GPU
- Model Deployment
- Serverless
- OpenAI Compatible
- Embeddings
- MLOps
---
