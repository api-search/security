---
api_key_in:
- query
api_specs:
- filename: crescendo-platform-openapi-original.json
  format: json
  label: Crescendo Platform API
  slug: crescendo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo/refs/heads/main/openapi/crescendo-platform-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Crescendo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crescendo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crescendo
provider_slug: crescendo
scheme_count: 2
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/crescendo-platform-openapi-original.json
  type: http
- description: Alternative to the Authorization header. Prefer the Authorization header whenever possible.
  in: query
  name: bearerTokenQuery
  parameter: bearer_token
  sources:
  - openapi/crescendo-platform-openapi-original.json
  type: apiKey
slug: crescendo-authentication
source_filename: crescendo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/crescendo-platform-openapi-original.json\ndocs: https://docs.crescendo.ai/api-reference/introduction\nnotes: >\n  Bearer API key. Send `Authorization: Bearer $CRESCENDO_API_KEY` (preferred) or\n  `?bearer_token=$CRESCENDO_API_KEY`. API keys are tenant-scoped and carry\n  prefix:resource.action scopes (e.g. provisioning:users.read, mcp:bots.*).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/crescendo-platform-openapi-original.json\n- name: bearerTokenQuery\n  type: apiKey\n  in: query\n  parameter: bearer_token\n  description: Alternative to the Authorization header. Prefer the Authorization header whenever\n    possible.\n  sources:\n  - openapi/crescendo-platform-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crescendo/refs/heads/main/authentication/crescendo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Customer Experience
- Customer Support
- Artificial Intelligence
- AI Agents
- Contact Center
- Conversational AI
- Voice of Customer
- MCP
---
