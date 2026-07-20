---
api_key_in:
- header
api_specs:
- filename: pioneer-openapi-original.json
  format: json
  label: Pioneer Inference API
  slug: pioneer-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastino-labs/refs/heads/main/openapi/pioneer-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fastino Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fastino Labs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fastino Labs
provider_slug: fastino-labs
scheme_count: 2
schemes:
- description: Pioneer API key. Generate one at https://agent.pioneer.ai/settings/api-keys. Keys begin with `pio_sk_`.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/pioneer-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  description: Supabase access token or Pioneer API key as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pioneer-openapi-original.json
  type: http
slug: fastino-labs-authentication
source_filename: fastino-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/pioneer-openapi-original.json\ndocs: https://docs.pioneer.ai/api-reference/authentication\nkey_prefix: pio_sk_\nkey_management:\n  create: POST https://api.pioneer.ai/create-api-key\n  list: GET https://api.pioneer.ai/list-api-keys\n  revoke: DELETE https://api.pioneer.ai/delete-api-key\n  console: https://agent.pioneer.ai/settings/api-keys\noauth:\n  provider: Supabase\n  metadata: https://api.pioneer.ai/.well-known/openid-configuration\n  scopes: scopes/fastino-labs-scopes.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Pioneer API key. Generate one at https://agent.pioneer.ai/settings/api-keys.\n    Keys begin with `pio_sk_`.\n  sources:\n  - openapi/pioneer-openapi-original.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Supabase access token or\
  \ Pioneer API key as a Bearer token.\n  sources:\n  - openapi/pioneer-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastino-labs/refs/heads/main/authentication/fastino-labs-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Small Language Models
- Fine-Tuning
- Inference
- Named Entity Recognition
- Information Extraction
- LLM
- Agents
- PII Detection
- Model Training
---
