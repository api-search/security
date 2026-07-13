---
api_key_in: []
api_specs:
- filename: parasail-inference-api-openapi.yml
  format: yaml
  label: Parasail Inference API
  slug: parasail-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/openapi/parasail-inference-api-openapi.yml
- filename: parasail-batch-api-openapi.yml
  format: yaml
  label: Parasail Batch API
  slug: parasail-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/openapi/parasail-batch-api-openapi.yml
- filename: parasail-dedicated-api-openapi.yml
  format: yaml
  label: Parasail Dedicated Deployments API
  slug: parasail-dedicated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/openapi/parasail-dedicated-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Parasail Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parasail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parasail
provider_slug: parasail
scheme_count: 1
schemes:
- description: Send your Parasail API key as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/parasail-batch-api-openapi.yml
  - openapi/parasail-dedicated-api-openapi.yml
  - openapi/parasail-inference-api-openapi.yml
  type: http
slug: parasail-ai-authentication
source_filename: parasail-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parasail-batch-api-openapi.yml, openapi/parasail-dedicated-api-openapi.yml,\n  openapi/parasail-inference-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Send your Parasail API key as a Bearer token.\n  sources:\n  - openapi/parasail-batch-api-openapi.yml\n  - openapi/parasail-dedicated-api-openapi.yml\n  - openapi/parasail-inference-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parasail/refs/heads/main/authentication/parasail-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- GPU
- Inference
- Large Language Models
- Open Source Models
- Hugging Face
- Batch
- Embeddings
- Tokenmaxxing
- Supercloud
---
