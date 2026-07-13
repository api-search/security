---
api_key_in: []
api_specs:
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Chat Completions API
  slug: featherless-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Completions API
  slug: featherless-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Models API
  slug: featherless-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Embeddings API
  slug: featherless-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Featherless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Featherless AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Featherless AI
provider_slug: featherless
scheme_count: 1
schemes:
- bearerFormat: Featherless API key
  description: 'Set `Authorization: Bearer <FEATHERLESS_API_KEY>`. Keys are created in the Featherless dashboard.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/featherless-openapi.yml
  type: http
slug: featherless-authentication
source_filename: featherless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/featherless-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Featherless API key\n  description: 'Set `Authorization: Bearer <FEATHERLESS_API_KEY>`. Keys are created in the Featherless\n    dashboard.'\n  sources:\n  - openapi/featherless-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/authentication/featherless-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Serverless
- Open Models
---
