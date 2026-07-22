---
api_key_in:
- query
api_specs:
- filename: primitive-openapi-original.json
  format: json
  label: Primitive API
  slug: primitive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Primitive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Primitive secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Primitive
provider_slug: primitive
scheme_count: 2
schemes:
- description: 'API key with `prim_` prefix or OAuth access token with `prim_oat_` prefix: `Authorization: Bearer <token>`. Access is governed by the caller''s organization role (`owner`, `admin`, or `member`): API keys always act at `member` level regardless of who created them, and OAuth access tokens act with the authorizing user''s current organization role, resolved per request. Every operation in this spec is'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/primitive-openapi-original.json
  type: http
- description: Signed download token provided in webhook payloads
  in: query
  name: DownloadToken
  parameter: token
  sources:
  - openapi/primitive-openapi-original.json
  type: apiKey
slug: primitive-authentication
source_filename: primitive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/primitive-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key with `prim_` prefix or OAuth access token with `prim_oat_` prefix: `Authorization:\n    Bearer <token>`. Access is governed by the caller''s organization role (`owner`, `admin`,\n    or `member`): API keys always act at `member` level regardless of who created them, and\n    OAuth access tokens act with the authorizing user''s current organization role, resolved\n    per request. Every operation in this spec is'\n  sources:\n  - openapi/primitive-openapi-original.json\n- name: DownloadToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Signed download token provided in webhook payloads\n  sources:\n  - openapi/primitive-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/authentication/primitive-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email
- Email Infrastructure
- AI Agents
- Agent Infrastructure
- Messaging
- Webhooks
- MCP
- Developer Tools
- API
---
