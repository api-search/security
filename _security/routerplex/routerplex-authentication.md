---
api_key_in: []
api_specs:
- filename: routerplex-chat-api-openapi.yml
  format: yaml
  label: RouterPlex Chat API
  slug: routerplex-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-chat-api-openapi.yml
- filename: routerplex-images-api-openapi.yml
  format: yaml
  label: RouterPlex Images API
  slug: routerplex-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-images-api-openapi.yml
- filename: routerplex-messages-api-openapi.yml
  format: yaml
  label: RouterPlex Messages API
  slug: routerplex-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-messages-api-openapi.yml
- filename: routerplex-models-api-openapi.yml
  format: yaml
  label: RouterPlex Models API
  slug: routerplex-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-models-api-openapi.yml
- filename: routerplex-responses-api-openapi.yml
  format: yaml
  label: RouterPlex Responses API
  slug: routerplex-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-responses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Routerplex Authentication
name_suffix: Authentication
oauth_flows: []
overview: RouterPlex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RouterPlex
provider_slug: routerplex
scheme_count: 1
schemes:
- bearerFormat: RouterPlex API key
  description: Create and manage API keys in the RouterPlex dashboard.
  name: RouterPlexApiKey
  scheme: bearer
  sources:
  - openapi/routerplex-inference-openapi.json
  type: http
slug: routerplex-authentication
source_filename: routerplex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/routerplex-inference-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: RouterPlexApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: RouterPlex API key\n  description: Create and manage API keys in the RouterPlex dashboard.\n  sources:\n  - openapi/routerplex-inference-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/authentication/routerplex-authentication.yml
summary_line: http · 1 scheme
tags:
- llm
- ai
- ai-gateway
- inference
- model-router
- openai-compatible
- anthropic-compatible
- claude
- gpt
- gemini
- api-gateway
- agent-infrastructure
- developer-tools
- mcp
- llmops
---
