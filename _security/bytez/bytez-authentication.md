---
api_key_in:
- header
api_specs:
- filename: bytez-openapi.yaml
  format: yaml
  label: Bytez Model API
  slug: bytez-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytez/refs/heads/main/openapi/bytez-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bytez Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bytez secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bytez
provider_slug: bytez
scheme_count: 1
schemes:
- description: "Set `Authorization` header to `BYTEZ_KEY` \n``` 'Authorization: YOUR_KEY_HERE' ```"
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/bytez-openapi.yaml
  type: apiKey
slug: bytez-authentication
source_filename: bytez-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bytez-openapi.yaml\ndocs: https://docs.bytez.com/model-api/docs/get-started\nnotes: >-\n  Single API key model. Send the Bytez key in the `Authorization` header (value\n  is the raw key, e.g. `Authorization: BYTEZ_KEY`). To call closed-source\n  providers (OpenAI, Anthropic, Cohere, Google, Mistral) add a second\n  `provider-key` header carrying your provider account key; Bytez pass-through\n  routes it and never stores it. Keys are issued from the API dashboard at\n  https://bytez.com/api. No OAuth / scopes surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"Set `Authorization` header to `BYTEZ_KEY` \\n``` 'Authorization: YOUR_KEY_HERE'\\\n    \\ ```\"\n  sources:\n  - openapi/bytez-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytez/refs/heads/main/authentication/bytez-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Model Inference
- LLM
- Open Source AI
- API
- Developers
---
