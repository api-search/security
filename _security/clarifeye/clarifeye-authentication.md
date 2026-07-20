---
api_key_in:
- header
api_specs:
- filename: clarifeye-openapi-original.yaml
  format: yaml
  label: Clarifeye Platform API — Public
  slug: clarifeye-platform-api-public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-openapi-original.yaml
- filename: clarifeye-backoffice-openapi-original.yaml
  format: yaml
  label: Clarifeye Platform API — Backoffice
  slug: clarifeye-platform-api-backoffice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/openapi/clarifeye-backoffice-openapi-original.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Clarifeye Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Clarifeye secures its APIs with apiKey, http, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Clarifeye
provider_slug: clarifeye
scheme_count: 2
schemes:
- description: 'Use Authorization: Bearer <token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/clarifeye-backoffice-openapi-original.yaml
  - openapi/clarifeye-openapi-original.yaml
  type: http
- description: 'Use Authorization: Token <token>'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/clarifeye-backoffice-openapi-original.yaml
  - openapi/clarifeye-openapi-original.yaml
  type: apiKey
slug: clarifeye-authentication
source_filename: clarifeye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clarifeye-backoffice-openapi-original.yaml, openapi/clarifeye-openapi-original.yaml\ndocs: https://docs.clarifeye.ai/guides/mcp-authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  notes: >\n    REST API uses a user token sent as either `Authorization: Bearer <token>`\n    or `Authorization: Token <token>`. The hosted MCP server additionally\n    supports OAuth 2.0 (authorizationCode + PKCE S256, Dynamic Client\n    Registration) with scopes claudeai / openid / offline_access. See\n    scopes/clarifeye-scopes.yml.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Use Authorization: Bearer <token>'\n  sources:\n  - openapi/clarifeye-backoffice-openapi-original.yaml\n  - openapi/clarifeye-openapi-original.yaml\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Use\
  \ Authorization: Token <token>'\n  sources:\n  - openapi/clarifeye-backoffice-openapi-original.yaml\n  - openapi/clarifeye-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarifeye/refs/heads/main/authentication/clarifeye-authentication.yml
summary_line: apiKey/http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Knowledge Management
- Model Context Protocol
- Document Intelligence
- Agents
- Enterprise AI
- Retrieval
---
