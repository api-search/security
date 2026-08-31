---
api_key_in:
- header
api_specs:
- filename: tl-dv-meetings-api-openapi.yml
  format: yaml
  label: tl;dv Meetings API
  slug: tl-dv-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-meetings-api-openapi.yml
- filename: tl-dv-notes-api-openapi.yml
  format: yaml
  label: tl;dv Notes API
  slug: tl-dv-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-notes-api-openapi.yml
- filename: tl-dv-system-api-openapi.yml
  format: yaml
  label: tl;dv System API
  slug: tl-dv-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-system-api-openapi.yml
- filename: tl-dv-transcripts-api-openapi.yml
  format: yaml
  label: tl;dv Transcripts API
  slug: tl-dv-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-transcripts-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tl Dv Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: tl;dv secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: tl;dv
provider_slug: tl-dv
scheme_count: 2
schemes:
- description: 'All requests authenticate with an API key sent on the x-api-key header. Keys are issued per user from tl;dv account settings and can be scoped to user, team, or organization context.

    '
  in: header
  key_management_url: https://tldv.io/app/settings/personal-settings/api-keys
  name: ApiKeyAuth
  parameter: x-api-key
  plan_requirement: Business or Enterprise tl;dv account
  plan_requirement_source: https://github.com/tldv-public/tldv-mcp-server
  sources:
  - openapi/tl-dv-openapi.yml
  surface: rest
  type: apiKey
- description: 'The hosted MCP endpoint https://mcp.tldv.io/mcp is protected by OAuth 2.1 with PKCE (S256) against a Keycloak realm, advertised via RFC 9728 protected-resource metadata and RFC 8414 authorization-server metadata. Discovered by probe on 2026-08-14; not documented by tl;dv anywhere. Dynamic client registration is open. A single coarse scope, mcp:tools, grants every tool.

    '
  dynamic_client_registration: https://keycloak.tldv.io/realms/mcp.tldv.io/clients-registrations/openid-connect
  flows:
  - authorizationUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/auth
    flow: authorizationCode
    scopes:
    - mcp:tools
    tokenUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token
  issuer: https://keycloak.tldv.io/realms/mcp.tldv.io
  method: probed
  name: MCPOAuth
  pkce: S256
  see: scopes/tl-dv-scopes.yml
  sources:
  - well-known/tl-dv-oauth-protected-resource.json
  - well-known/tl-dv-oauth-authorization-server.json
  surface: mcp
  type: oauth2
slug: tl-dv-authentication
source_filename: tl-dv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://doc.tldv.io\ndocs: https://doc.tldv.io\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_names: [x-api-key]\n  oauth2_flows: [authorizationCode]\n  note: >\n    Two DIFFERENT auth models on two different surfaces. The REST API is\n    api-key only. The hosted MCP endpoint added on 2026-08-14 is OAuth 2.1\n    against a Keycloak realm. They are not interchangeable: an x-api-key will\n    not authenticate mcp.tldv.io, and an OAuth token will not authenticate\n    pasta.tldv.io.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >\n      All requests authenticate with an API key sent on the x-api-key header.\n      Keys are issued per user from tl;dv account settings and can be scoped to\n      user, team, or organization context.\n    key_management_url: https://tldv.io/app/settings/personal-settings/api-keys\n    sources: [openapi/tl-dv-openapi.yml]\n\
  \    surface: rest\n    plan_requirement: Business or Enterprise tl;dv account\n    plan_requirement_source: https://github.com/tldv-public/tldv-mcp-server\n  - name: MCPOAuth\n    type: oauth2\n    surface: mcp\n    method: probed\n    description: >\n      The hosted MCP endpoint https://mcp.tldv.io/mcp is protected by OAuth 2.1\n      with PKCE (S256) against a Keycloak realm, advertised via RFC 9728\n      protected-resource metadata and RFC 8414 authorization-server metadata.\n      Discovered by probe on 2026-08-14; not documented by tl;dv anywhere.\n      Dynamic client registration is open. A single coarse scope, mcp:tools,\n      grants every tool.\n    issuer: https://keycloak.tldv.io/realms/mcp.tldv.io\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/auth\n        tokenUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token\n        scopes: [mcp:tools]\n    pkce:\
  \ S256\n    dynamic_client_registration: https://keycloak.tldv.io/realms/mcp.tldv.io/clients-registrations/openid-connect\n    sources:\n      - well-known/tl-dv-oauth-protected-resource.json\n      - well-known/tl-dv-oauth-authorization-server.json\n    see: scopes/tl-dv-scopes.yml\nnotes: >\n  The REST API uses a single API-key model with no scope surface. An OAuth2\n  scope surface DOES exist, but only on the hosted MCP endpoint, so\n  scopes/tl-dv-scopes.yml is scoped to that surface. Health check (GET\n  /v1alpha1/health) is the only unauthenticated REST operation; it was probed\n  anonymously on 2026-08-14 and returned 200 {\"status\":\"ok\"}. API access\n  requires a Business or Enterprise account regardless of surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/authentication/tl-dv-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Meetings
- Transcription
- Notetaking
- Conversation Intelligence
- Productivity
- Video
- Webhook
---
