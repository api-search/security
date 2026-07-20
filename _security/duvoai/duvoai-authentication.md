---
api_key_in:
- header
api_specs:
- filename: duvoai-openapi-original.json
  format: json
  label: Duvo Public API
  slug: duvo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duvoai/refs/heads/main/openapi/duvoai-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Duvoai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: duvo.ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: duvo.ai
provider_slug: duvoai
scheme_count: 2
schemes:
- description: 'Workspace-issued API key presented as `Authorization: Bearer <token>`. Keys are provisioned through Duvo customer onboarding (no self-serve registration) and stored via `duvo login` or the `DUVO_API_KEY` environment variable.'
  header: 'Authorization: Bearer <token>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/duvoai-openapi-original.json
  type: http
- authorization_server: https://login.duvo.ai/
  description: 'Enterprise workspaces with OAuth enabled request an access token from the configured authorization server and present it as `Authorization: Bearer <access_token>`. Authorization-server metadata is discoverable at the RFC 8414 well-known endpoint.'
  name: enterpriseOAuth
  scheme: clientCredentials
  sources:
  - docs:https://www.duvo.ai/auth.md
  - well-known/duvoai-oauth-authorization-server.json
  token_endpoint: https://login.duvo.ai/oauth/token
  type: oauth2
  well_known: https://login.duvo.ai/.well-known/oauth-authorization-server
slug: duvoai-authentication
source_filename: duvoai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/duvoai-openapi-original.json\ndocs: https://www.duvo.ai/auth.md\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Workspace-issued API key presented as `Authorization: Bearer <token>`.\n    Keys are provisioned through Duvo customer onboarding (no self-serve\n    registration) and stored via `duvo login` or the `DUVO_API_KEY`\n    environment variable.\n  header: 'Authorization: Bearer <token>'\n  sources:\n  - openapi/duvoai-openapi-original.json\n- name: enterpriseOAuth\n  type: oauth2\n  scheme: clientCredentials\n  description: >-\n    Enterprise workspaces with OAuth enabled request an access token from the\n    configured authorization server and present it as\n    `Authorization: Bearer <access_token>`. Authorization-server metadata is\n    discoverable at the RFC 8414\
  \ well-known endpoint.\n  authorization_server: https://login.duvo.ai/\n  well_known: https://login.duvo.ai/.well-known/oauth-authorization-server\n  token_endpoint: https://login.duvo.ai/oauth/token\n  sources:\n  - docs:https://www.duvo.ai/auth.md\n  - well-known/duvoai-oauth-authorization-server.json\nnotes:\n- 401 indicates a credential problem; 403 signals insufficient scope or policy denial (error code `insufficient_scope`).\n- Scope reference captured in scopes/duvoai-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duvoai/refs/heads/main/authentication/duvoai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai Ml
- Process Intelligence
- Automation
- Agents
- MCP
- Enterprise Operations
- SAP Migration
- Workflow
---
