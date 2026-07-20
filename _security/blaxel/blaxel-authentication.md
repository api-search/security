---
api_key_in:
- header
api_specs:
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Agents API
  slug: blaxel-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Functions / MCP Servers API
  slug: blaxel-functions-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Models Gateway API
  slug: blaxel-models-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Sandboxes API
  slug: blaxel-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Jobs API
  slug: blaxel-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Policies API
  slug: blaxel-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Integrations API
  slug: blaxel-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Workspaces API
  slug: blaxel-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Blaxel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blaxel secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blaxel
provider_slug: blaxel
scheme_count: 2
schemes:
- description: API key supplied as "Bearer [example key]".
  in: header
  name: apiKey
  parameter: X-Blaxel-Authorization
  sources:
  - openapi/blaxel-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 short-lived JWT access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blaxel-openapi.yml
  type: http
slug: blaxel-authentication
source_filename: blaxel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blaxel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Blaxel-Authorization\n  description: API key supplied as \"Bearer [example key]\".\n  sources:\n  - openapi/blaxel-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 short-lived JWT access token.\n  sources:\n  - openapi/blaxel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/authentication/blaxel-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Agents
- Infrastructure
- Sandboxes
- MCP
- Compute
- Serverless
---
