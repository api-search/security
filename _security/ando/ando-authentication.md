---
api_key_in:
- header
api_specs:
- filename: ando-public-api-v1-openapi.json
  format: json
  label: Ando Public API v1
  slug: ando-public-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/openapi/ando-public-api-v1-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ando Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ando secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ando
provider_slug: ando
scheme_count: 2
schemes:
- description: Workspace API key. Current accepted keys use the ando_sk_ prefix.
  in: header
  name: AndoApiKey
  parameter: x-api-key
  sources:
  - openapi/ando-public-api-v1-openapi.json
  type: apiKey
- bearerFormat: ando_sk
  description: Compatibility transport for workspace API keys.
  name: BearerApiKey
  scheme: bearer
  sources:
  - openapi/ando-public-api-v1-openapi.json
  type: http
slug: ando-authentication
source_filename: ando-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/ando-public-api-v1-openapi.json\ndocs: https://docs.ando.so/api-reference/authorization\nnotes: >-\n  Server-side workspace API keys with the ando_sk_ prefix, created in Settings ->\n  API keys. Send via the x-api-key header (preferred) or Authorization: Bearer\n  for compatibility with older clients. Each key is scoped to one workspace and\n  Ando derives authorship from the key or connected-agent identity. Third-party\n  agent keys and workspace/service keys are additional actor variants of the same\n  API-key model. No OAuth surface (no scopes artifact).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AndoApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Workspace API key. Current accepted keys use the ando_sk_ prefix.\n  sources:\n  - openapi/ando-public-api-v1-openapi.json\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ando_sk\n\
  \  description: Compatibility transport for workspace API keys.\n  sources:\n  - openapi/ando-public-api-v1-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ando/refs/heads/main/authentication/ando-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Business Applications
- Messaging
- Team Collaboration
- AI Agents
- Agents
- Developer Tools
- MCP
- Webhooks
- Productivity
---
