---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: OpenRouter
  slug: openrouter
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Chat Completions API
  slug: chat-completions-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Generation API
  slug: generation-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Keys Management API
  slug: keys-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openrouter Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenRouter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenRouter
provider_slug: openrouter
scheme_count: 1
schemes:
- bearerFormat: OPENROUTER_API_KEY
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openrouter-openapi.yml
  type: http
slug: openrouter-authentication
source_filename: openrouter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openrouter-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OPENROUTER_API_KEY\n  sources:\n  - openapi/openrouter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/authentication/openrouter-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Gateway
- Large Language Models
- Router
---
