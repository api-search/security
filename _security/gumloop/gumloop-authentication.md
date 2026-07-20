---
api_key_in: []
api_specs:
- filename: gumloop-openapi-original.yml
  format: yaml
  label: Gumloop Public API
  slug: gumloop-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gumloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gumloop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gumloop
provider_slug: gumloop
scheme_count: 1
schemes:
- description: A personal API key or an [OAuth 2.0](/api-reference/oauth) access token. Personal API keys also require the `x-auth-key` header with your user ID.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gumloop-openapi-original.yml
  type: http
slug: gumloop-authentication
source_filename: gumloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gumloop-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A personal API key or an [OAuth 2.0](/api-reference/oauth) access token. Personal\n    API keys also require the `x-auth-key` header with your user ID.\n  sources:\n  - openapi/gumloop-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/authentication/gumloop-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Workflow Automation
- Agent Platform
- MCP
- LLM
- No-Code
- Developer Tools
---
