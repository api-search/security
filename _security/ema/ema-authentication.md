---
api_key_in:
- header
auth_types:
- apiKey
- http
description: Ema's Builder Platform API uses a two-step authentication flow. First an API key is generated for a user within a specific tenant via the gRPC-Web endpoint auth.v1.AuthService/GenerateApiKey. That long-lived API key is then exchanged for a short-lived JWT access token via a REST call. All subsequent REST and gRPC-Web calls carry the access token as an HTTP Bearer token in the Authorization header. Ema is multi-tenant; keys and tokens are scoped to a tenant and user.
kind: authentication
layout: security
method: searched
name: Ema Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ema secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ema
provider_slug: ema
scheme_count: 2
schemes:
- in: header
  issued_by: auth.v1.AuthService/GenerateApiKey (gRPC-Web)
  lifetime: long-lived
  name: apiKey
  parameter: x-ema-api-key
  source: https://builder.ema.ai/api-reference/authentication
  type: apiKey
  used_for: exchanged at POST /api/auth/generate_access_token to mint an access token
- bearer_format: JWT
  in: header
  lifetime: short-lived (access token)
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  source: https://builder.ema.ai/api-reference/authentication
  type: http
  used_for: all REST and gRPC-Web API calls
slug: ema-authentication
source_filename: ema-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://builder.ema.ai/api-reference/authentication\ndocs: https://builder.ema.ai/api-reference/authentication\nsummary:\n  model: two-step api-key then short-lived JWT bearer\n  types: [apiKey, http]\n  api_key_in: [header]\n  bearer_format: JWT\ndescription: >-\n  Ema's Builder Platform API uses a two-step authentication flow. First an API\n  key is generated for a user within a specific tenant via the gRPC-Web endpoint\n  auth.v1.AuthService/GenerateApiKey. That long-lived API key is then exchanged\n  for a short-lived JWT access token via a REST call. All subsequent REST and\n  gRPC-Web calls carry the access token as an HTTP Bearer token in the\n  Authorization header. Ema is multi-tenant; keys and tokens are scoped to a\n  tenant and user.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-ema-api-key\n  used_for: exchanged at POST /api/auth/generate_access_token to mint an access token\n  issued_by:\
  \ auth.v1.AuthService/GenerateApiKey (gRPC-Web)\n  lifetime: long-lived\n  source: https://builder.ema.ai/api-reference/authentication\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  parameter: Authorization\n  used_for: all REST and gRPC-Web API calls\n  lifetime: short-lived (access token)\n  source: https://builder.ema.ai/api-reference/authentication\nflow:\n- step: 1\n  action: GenerateApiKey\n  protocol: gRPC-Web over HTTP\n  endpoint: /auth.v1.AuthService/GenerateApiKey\n  note: >-\n    For the first request (root tenant, no token yet) the browser session\n    bearer token can be reused once; see\n    https://builder.ema.ai/api-reference/misc/root-tenant-token\n- step: 2\n  action: GenerateAccessToken\n  protocol: REST\n  endpoint: POST /api/auth/generate_access_token\n  request_header: 'x-ema-api-key: <api-key>'\n  returns: JWT access token (short-lived)\n- step: 3\n  action: authenticated calls\n  header: 'Authorization: Bearer <access_token>'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ema/refs/heads/main/authentication/ema-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Agents
- AI Employees
- Automation
- Enterprise
- Workflow Automation
- Conversational AI
---
