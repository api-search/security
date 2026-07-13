---
api_key_in: []
api_specs:
- filename: prime-intellect-compute-api-openapi.yml
  format: yaml
  label: Prime Intellect Compute API
  slug: prime-intellect-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-compute-api-openapi.yml
- filename: prime-intellect-sandbox-api-openapi.yml
  format: yaml
  label: Prime Intellect Sandbox API
  slug: prime-intellect-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-sandbox-api-openapi.yml
- filename: prime-intellect-training-api-openapi.yml
  format: yaml
  label: Prime Intellect Training API
  slug: prime-intellect-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-training-api-openapi.yml
- filename: prime-intellect-evaluations-api-openapi.yml
  format: yaml
  label: Prime Intellect Evaluations API
  slug: prime-intellect-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-evaluations-api-openapi.yml
- filename: prime-intellect-inference-api-openapi.yml
  format: yaml
  label: Prime Intellect Inference API
  slug: prime-intellect-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-inference-api-openapi.yml
- filename: prime-intellect-platform-api-openapi.yml
  format: yaml
  label: Prime Intellect Platform API
  slug: prime-intellect-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prime Intellect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prime Intellect secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prime Intellect
provider_slug: prime-intellect
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/prime-intellect-compute-api-openapi.yml
  - openapi/prime-intellect-evaluations-api-openapi.yml
  - openapi/prime-intellect-inference-api-openapi.yml
  - openapi/prime-intellect-platform-api-openapi.yml
  - openapi/prime-intellect-sandbox-api-openapi.yml
  - openapi/prime-intellect-training-api-openapi.yml
  type: http
slug: prime-intellect-authentication
source_filename: prime-intellect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prime-intellect-compute-api-openapi.yml, openapi/prime-intellect-evaluations-api-openapi.yml,\n  openapi/prime-intellect-inference-api-openapi.yml, openapi/prime-intellect-platform-api-openapi.yml,\n  openapi/prime-intellect-sandbox-api-openapi.yml, openapi/prime-intellect-training-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/prime-intellect-compute-api-openapi.yml\n  - openapi/prime-intellect-evaluations-api-openapi.yml\n  - openapi/prime-intellect-inference-api-openapi.yml\n  - openapi/prime-intellect-platform-api-openapi.yml\n  - openapi/prime-intellect-sandbox-api-openapi.yml\n  - openapi/prime-intellect-training-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/authentication/prime-intellect-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Reinforcement Learning
- GPU Compute
- Decentralized Compute
- Foundation Models
- Inference
- Sandboxes
- Training
- Environments
- Evaluations
- LoRA
- Open Source
- Agents
---
