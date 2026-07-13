---
api_key_in: []
api_specs:
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes LLM Inference (Chat Completions) API
  slug: chutes-llm-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes Image / Other Models API
  slug: chutes-image-other-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes Management (Deploy / List) API
  slug: chutes-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes Images API
  slug: chutes-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chutes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chutes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chutes
provider_slug: chutes
scheme_count: 1
schemes:
- description: 'Chutes API key passed as `Authorization: Bearer cpk_...`. Management endpoints alternatively accept a Bittensor hotkey signature (X-Chutes-Hotkey, X-Chutes-Signature, X-Chutes-Nonce).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chutes-openapi.yml
  type: http
slug: chutes-authentication
source_filename: chutes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chutes-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Chutes API key passed as `Authorization: Bearer cpk_...`. Management endpoints\n    alternatively accept a Bittensor hotkey signature (X-Chutes-Hotkey, X-Chutes-Signature,\n    X-Chutes-Nonce).'\n  sources:\n  - openapi/chutes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/authentication/chutes-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Serverless
- GPU
- Bittensor
---
