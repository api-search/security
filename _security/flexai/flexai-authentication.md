---
api_key_in: []
api_specs:
- filename: flexai-token-factory-openapi.yml
  format: yaml
  label: FlexAI Token Factory API
  slug: flexai-token-factory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-token-factory-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flexai Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlexAI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FlexAI
provider_slug: flexai
scheme_count: 1
schemes:
- description: 'FlexAI API key passed as a bearer token: `Authorization: Bearer $FLEXAI_API_KEY`. Create a key at https://tokens.flex.ai/signup.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flexai-token-factory-openapi.yml
  type: http
slug: flexai-authentication
source_filename: flexai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/flexai-token-factory-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'FlexAI API key passed as a bearer token: `Authorization: Bearer $FLEXAI_API_KEY`.\n    Create a key at https://tokens.flex.ai/signup.'\n  sources:\n  - openapi/flexai-token-factory-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/authentication/flexai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai/Ml
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- Large Language Models
- OpenAI Compatible
- GPU Compute
- Embeddings
- Fine-Tuning
- Agents
---
