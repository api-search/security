---
api_key_in:
- header
api_specs:
- filename: sahara-ai-compute-openapi.yml
  format: yaml
  label: Sahara AI Compute API
  slug: sahara-ai-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahara-ai/refs/heads/main/openapi/sahara-ai-compute-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sahara Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sahara AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sahara AI
provider_slug: sahara-ai
scheme_count: 2
schemes:
- description: API key issued from the Developer Portal. Passed in the `x-api-key` header. Never expose your API key in public code or repositories.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/sahara-ai-compute-openapi.yml
  type: apiKey
- description: API key passed as a Bearer token in the Authorization header (OpenAI-compatible clients).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sahara-ai-compute-openapi.yml
  type: http
slug: sahara-ai-authentication
source_filename: sahara-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sahara-ai-compute-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued from the Developer Portal. Passed in the `x-api-key` header. Never\n    expose your API key in public code or repositories.\n  sources:\n  - openapi/sahara-ai-compute-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header (OpenAI-compatible\n    clients).\n  sources:\n  - openapi/sahara-ai-compute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sahara-ai/refs/heads/main/authentication/sahara-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crypto
- Artificial Intelligence
- Machine Learning
- Agents
- Compute
- Blockchain
- Inference
- Data
---
