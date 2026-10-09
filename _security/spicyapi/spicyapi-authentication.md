---
anonymous_access: false
api_key_in: []
api_specs:
- filename: spicyapi-account-api-openapi.yml
  format: yaml
  label: SpicyAPI Account API
  slug: spicyapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-account-api-openapi.yml
- filename: spicyapi-media-api-openapi.yml
  format: yaml
  label: SpicyAPI Media API
  slug: spicyapi-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-media-api-openapi.yml
- filename: spicyapi-models-api-openapi.yml
  format: yaml
  label: SpicyAPI Models API
  slug: spicyapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-models-api-openapi.yml
- filename: spicyapi-openai-compatible-api-openapi.yml
  format: yaml
  label: SpicyAPI OpenAI Compatible API
  slug: spicyapi-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-openai-compatible-api-openapi.yml
- filename: spicyapi-tasks-api-openapi.yml
  format: yaml
  label: SpicyAPI Tasks API
  slug: spicyapi-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Spicyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpicyAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpicyAPI
provider_slug: spicyapi
scheme_count: 1
schemes:
- bearerFormat: sk-spicy-<48 lowercase hex characters>
  description: 'Send `Authorization: Bearer sk-spicy-...`. Keep keys server-side.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spicyapi-openapi.yml
  type: http
slug: spicyapi-authentication
source_filename: spicyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/spicyapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk-spicy-<48 lowercase hex characters>\n  description: 'Send `Authorization: Bearer sk-spicy-...`. Keep keys server-side.'\n  sources:\n  - openapi/spicyapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/authentication/spicyapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative Media
- LLM
- Video Generation
- Image Generation
- Model Aggregator
---
