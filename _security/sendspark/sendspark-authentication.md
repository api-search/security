---
api_key_in:
- header
api_specs:
- filename: sendspark-openapi-original.json
  format: json
  label: Sendspark API
  slug: sendspark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sendspark Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refresh_token
- device_code
overview: Sendspark secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refresh_token, and device_code flow(s).
provider_name: Sendspark
provider_slug: sendspark
scheme_count: 3
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/sendspark-openapi-original.json
  type: apiKey
- in: header
  name: apiSecret
  parameter: x-api-secret
  sources:
  - openapi/sendspark-openapi-original.json
  type: apiKey
- issuer: https://auth.sendspark.com
  metadata: https://apiv2.sendspark.com/.well-known/oauth-authorization-server
  name: mcpOAuth
  note: The hosted MCP server (apiv2.sendspark.com/api/mcp) authenticates over OAuth 2.0 via browser sign-in (issuer https://auth.sendspark.com), separate from the REST API's x-api-key/x-api-secret header auth.
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/sendspark-oauth-authorization-server.json
  type: oauth2
slug: sendspark-authentication
source_filename: sendspark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sendspark-openapi-original.json\ndocs: https://help.sendspark.com/api-reference\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refresh_token\n  - device_code\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/sendspark-openapi-original.json\n- name: apiSecret\n  type: apiKey\n  in: header\n  parameter: x-api-secret\n  sources:\n  - openapi/sendspark-openapi-original.json\n- name: mcpOAuth\n  type: oauth2\n  note: >-\n    The hosted MCP server (apiv2.sendspark.com/api/mcp) authenticates over OAuth 2.0\n    via browser sign-in (issuer https://auth.sendspark.com), separate from the REST\n    API's x-api-key/x-api-secret header auth.\n  issuer: https://auth.sendspark.com\n  metadata: https://apiv2.sendspark.com/.well-known/oauth-authorization-server\n  scopes_supported: [openid, profile, email, offline_access]\n\
  \  sources:\n  - well-known/sendspark-oauth-authorization-server.json\nnotes: >-\n  REST API calls require BOTH x-api-key and x-api-secret headers; keys are\n  workspace-scoped. GET /v1/workspaces/identifier resolves the workspace id for a\n  key pair.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/authentication/sendspark-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Video
- Sales
- Marketing
- Personalization
- Artificial Intelligence
- Video Messaging
- Webhooks
- MCP
---
