---
api_key_in: []
api_specs:
- filename: sail-batches-api-api-openapi.yml
  format: yaml
  label: Sail Batches API API
  slug: sail-batches-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/openapi/sail-batches-api-api-openapi.yml
- filename: sail-chat-completions-api-api-openapi.yml
  format: yaml
  label: Sail Chat Completions API API
  slug: sail-chat-completions-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/openapi/sail-chat-completions-api-api-openapi.yml
- filename: sail-messages-api-api-openapi.yml
  format: yaml
  label: Sail Messages API API
  slug: sail-messages-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/openapi/sail-messages-api-api-openapi.yml
- filename: sail-models-api-api-openapi.yml
  format: yaml
  label: Sail Models API API
  slug: sail-models-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/openapi/sail-models-api-api-openapi.yml
- filename: sail-responses-api-api-openapi.yml
  format: yaml
  label: Sail Responses API API
  slug: sail-responses-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/openapi/sail-responses-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sail
provider_slug: sail
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sail-openapi-original.json
  type: http
slug: sail-authentication
source_filename: sail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sail-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/sail-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/authentication/sail-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Machine Learning
- LLM
- Inference
- Agents
- Open Source Models
- Infrastructure
- Developer Tools
---
