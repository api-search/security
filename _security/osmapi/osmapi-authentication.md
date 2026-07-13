---
api_key_in: []
api_specs:
- filename: osmapi-chat-completions-openapi.yml
  format: yaml
  label: osmAPI Chat Completions API
  slug: osmapi-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-chat-completions-openapi.yml
- filename: osmapi-anthropic-messages-openapi.yml
  format: yaml
  label: osmAPI Anthropic Messages API
  slug: osmapi-anthropic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-anthropic-messages-openapi.yml
- filename: osmapi-models-openapi.yml
  format: yaml
  label: osmAPI Models API
  slug: osmapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-models-openapi.yml
- filename: osmapi-health-openapi.yml
  format: yaml
  label: osmAPI Health API
  slug: osmapi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Osmapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: osmAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: osmAPI
provider_slug: osmapi
scheme_count: 1
schemes:
- description: Bearer token using osmAPI key (osmint_XXXXXXXXXXXXXXXX)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/osmapi-anthropic-messages-openapi.yml
  - openapi/osmapi-chat-completions-openapi.yml
  type: http
slug: osmapi-authentication
source_filename: osmapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/osmapi-anthropic-messages-openapi.yml, openapi/osmapi-chat-completions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token using osmAPI key (osmint_XXXXXXXXXXXXXXXX)\n  sources:\n  - openapi/osmapi-anthropic-messages-openapi.yml\n  - openapi/osmapi-chat-completions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/authentication/osmapi-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Anthropic
- Gateway
- LLM
- OpenAI
- Routing
---
