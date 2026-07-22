---
api_key_in:
- header
api_specs:
- filename: txt-dottxt-openapi-original.json
  format: json
  label: dottxt API
  slug: dottxt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/txt/refs/heads/main/openapi/txt-dottxt-openapi-original.json
auth_types:
- http-bearer
description: 'Auth profile for the dottxt API, from the published OpenAPI securitySchemes (openapi/txt-dottxt-openapi-original.json) and the docs authentication page. Single scheme: bearer API key in the Authorization header. Keys are prefixed sk-dottxt- and are created/managed in the dashboard; access is currently granted via a request form. The Python SDK and CLI read DOTTXT_API_KEY by default (dottxt login stores credentials locally).'
kind: authentication
layout: security
method: searched
name: Txt Authentication
name_suffix: Authentication
oauth_flows: []
overview: .txt secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: .txt
provider_slug: txt
scheme_count: 1
schemes:
- bearerFormat: API Key
  environment_variable: DOTTXT_API_KEY
  header: 'Authorization: Bearer <DOTTXT_API_KEY>'
  key_prefix: sk-dottxt-
  name: BearerAuth
  notes: 'API keys can be created and managed in the dashboard. Connection check: GET https://api.dottxt.ai/v1/models with the bearer header returns 200 with the models available to the key. 401 = invalid/missing key, 403 = key lacks access to the requested model, 402 = insufficient credits.'
  scheme: bearer
  sources:
  - openapi/txt-dottxt-openapi-original.json
  type: http
slug: txt-authentication
source_filename: txt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.dottxt.ai/api/authentication\ndocs: https://docs.dottxt.ai/api/authentication\ndescription: >-\n  Auth profile for the dottxt API, from the published OpenAPI securitySchemes\n  (openapi/txt-dottxt-openapi-original.json) and the docs authentication page.\n  Single scheme: bearer API key in the Authorization header. Keys are prefixed\n  sk-dottxt- and are created/managed in the dashboard; access is currently\n  granted via a request form. The Python SDK and CLI read DOTTXT_API_KEY by\n  default (dottxt login stores credentials locally).\nsummary:\n  types: [http-bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: API Key\n    header: 'Authorization: Bearer <DOTTXT_API_KEY>'\n    key_prefix: sk-dottxt-\n    environment_variable: DOTTXT_API_KEY\n    sources: [openapi/txt-dottxt-openapi-original.json]\n    notes: >-\n      API keys\
  \ can be created and managed in the dashboard. Connection check:\n      GET https://api.dottxt.ai/v1/models with the bearer header returns 200\n      with the models available to the key. 401 = invalid/missing key, 403 =\n      key lacks access to the requested model, 402 = insufficient credits.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/txt/refs/heads/main/authentication/txt-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- Structured Outputs
- JSON Schema
- Inference
- Developer Tools
- Machine Learning
---
