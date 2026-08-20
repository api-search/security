---
api_key_in: []
api_specs:
- filename: glama-auth-api-openapi.yml
  format: yaml
  label: Glama AI Auth API
  slug: glama-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-auth-api-openapi.yml
- filename: glama-chat-completions-api-openapi.yml
  format: yaml
  label: Glama AI Chat Completions API
  slug: glama-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-chat-completions-api-openapi.yml
- filename: glama-models-api-openapi.yml
  format: yaml
  label: Glama AI Models API
  slug: glama-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-models-api-openapi.yml
- filename: glama-observability-api-openapi.yml
  format: yaml
  label: Glama AI Observability API
  slug: glama-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-observability-api-openapi.yml
- filename: glama-responses-api-openapi.yml
  format: yaml
  label: Glama AI Responses API
  slug: glama-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-responses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Glama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glama AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Glama AI
provider_slug: glama
scheme_count: 1
schemes:
- bearerFormat: Glama API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/glama-openapi.yml
  type: http
slug: glama-authentication
source_filename: glama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glama-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Glama API Key\n  sources:\n  - openapi/glama-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/authentication/glama-authentication.yml
summary_line: http · 1 scheme
tags:
- MCP
- MCP Marketplace
- MCP Gateway
- MCP Hosting
- MCP Inspector
- AI Gateway
- LLM Gateway
- Connectors
- Authentication
- Observability
- Multi-Provider
---
