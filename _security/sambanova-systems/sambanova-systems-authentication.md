---
api_key_in:
- header
api_specs:
- filename: sambanova-systems-cloud-openapi-original.yml
  format: yaml
  label: SambaNova Cloud API
  slug: sambanova-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-cloud-openapi-original.yml
- filename: sambanova-systems-agents-openapi-original.yml
  format: yaml
  label: SambaNova Agents Service
  slug: sambanova-agents-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-agents-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sambanova Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: SambaNova Systems secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SambaNova Systems
provider_slug: sambanova-systems
scheme_count: 2
schemes:
- bearerFormat: apiKey
  description: SambaNova API Key
  name: api_key
  scheme: bearer
  sources:
  - openapi/sambanova-systems-agents-openapi-original.yml
  - openapi/sambanova-systems-cloud-openapi-original.yml
  type: http
- description: SambaNova API key, sent in the `x-api-key` header. Accepted on the Messages API routes (`/messages`, `/messages/count_tokens`) so that callers can point the official Anthropic SDK at SambaNova by swapping `base_url` — no code changes. The credential value is the same as the bearer `api_key` scheme; only the transport differs.
  in: header
  name: x_api_key
  parameter: x-api-key
  sources:
  - openapi/sambanova-systems-cloud-openapi-original.yml
  type: apiKey
slug: sambanova-systems-authentication
source_filename: sambanova-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sambanova-systems-agents-openapi-original.yml, openapi/sambanova-systems-cloud-openapi-original.yml\ndocs: https://docs.sambanova.ai/cloud/docs/get-started/api-keys-urls\nnotes: >-\n  Authentication is a SambaNova API key generated in the SambaCloud portal (https://cloud.sambanova.ai/apis);\n  up to 25 keys per user. Sent as a bearer token (Authorization: Bearer <key>) on all OpenAI-compatible\n  routes, or as the x-api-key header on the Anthropic Messages API routes (/messages, /messages/count_tokens).\n  The credential value is identical across both transports. Keys cannot be viewed again after generation.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: SambaNova API Key\n  sources:\n  - openapi/sambanova-systems-agents-openapi-original.yml\n  - openapi/sambanova-systems-cloud-openapi-original.yml\n\
  - name: x_api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: SambaNova API key, sent in the `x-api-key` header. Accepted on the Messages API\n    routes (`/messages`, `/messages/count_tokens`) so that callers can point the official Anthropic\n    SDK at SambaNova by swapping `base_url` — no code changes. The credential value is the same\n    as the bearer `api_key` scheme; only the transport differs.\n  sources:\n  - openapi/sambanova-systems-cloud-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/authentication/sambanova-systems-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Generative AI
- API
- Agents
- Embeddings
---
