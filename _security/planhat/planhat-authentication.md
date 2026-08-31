---
api_key_in: []
auth_types:
- http
- oauth2
description: Planhat authenticates the main REST API with a bearer API access token (generated as a Private App under Settings; shown once, long-lived). Basic auth is also accepted. The remote MCP server and programmatic OAuth clients use OAuth 2.0 authorization_code + refresh_token with PKCE (S256) against api.planhat.com. The separate analytics/tracking endpoint is addressed by tenant UUID in the URL path (tenant-scoped, effectively open for ingest).
kind: authentication
layout: security
method: searched
name: Planhat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Planhat secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Planhat
provider_slug: planhat
scheme_count: 4
schemes:
- applies_to: https://api.planhat.com
  format: 'Authorization: Bearer {{apiAccessToken}}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://www.planhat.com/developers/api/authentication-limits
  token_source: Private App access token (Settings > Private Apps); appears once, store securely.
  type: http
- name: basicAuth
  note: Basic authentication is also accepted on the main API.
  scheme: basic
  sources:
  - https://www.planhat.com/developers/api/authentication-limits
  type: http
- client_id_prefix: pk_
  client_secret_prefix: sk_
  flows:
  - authorizationUrl: https://ws.planhat.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refresh: true
    scopes:
      inclusive: Broad inclusive scope (only scope advertised in RFC 8414 metadata).
    tokenUrl: https://api.planhat.com/oauth/token
  name: oauth2
  sources:
  - well-known/planhat-oauth-authorization-server.json
  - https://www.planhat.com/developers/ai/mcp-server/
  type: oauth2
  used_by: Remote MCP server (api.planhat.com/v1/mcp) and OAuth apps.
- in: path
  name: tenantUUID
  note: Analytics endpoint (analytics.planhat.com/analytics/{tenantUUID}) is addressed by tenant UUID in the path; Segment ingest uses Basic auth with tenantUUID as username. Not the main API auth.
  sources:
  - https://www.planhat.com/developers/api/user-activities
  type: apiKey
slug: planhat-authentication
source_filename: planhat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.planhat.com/developers/api/authentication-limits\ndocs: https://www.planhat.com/developers/api/authentication-limits\ndescription: >-\n  Planhat authenticates the main REST API with a bearer API access token\n  (generated as a Private App under Settings; shown once, long-lived). Basic auth\n  is also accepted. The remote MCP server and programmatic OAuth clients use\n  OAuth 2.0 authorization_code + refresh_token with PKCE (S256) against\n  api.planhat.com. The separate analytics/tracking endpoint is addressed by\n  tenant UUID in the URL path (tenant-scoped, effectively open for ingest).\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer, basic]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer {{apiAccessToken}}'\n  token_source: Private App access token (Settings > Private Apps);\
  \ appears once, store securely.\n  applies_to: https://api.planhat.com\n  sources: [https://www.planhat.com/developers/api/authentication-limits]\n- name: basicAuth\n  type: http\n  scheme: basic\n  note: Basic authentication is also accepted on the main API.\n  sources: [https://www.planhat.com/developers/api/authentication-limits]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ws.planhat.com/oauth/authorize\n    tokenUrl: https://api.planhat.com/oauth/token\n    pkce: S256\n    refresh: true\n    scopes:\n      inclusive: Broad inclusive scope (only scope advertised in RFC 8414 metadata).\n  client_id_prefix: pk_\n  client_secret_prefix: sk_\n  used_by: Remote MCP server (api.planhat.com/v1/mcp) and OAuth apps.\n  sources:\n  - well-known/planhat-oauth-authorization-server.json\n  - https://www.planhat.com/developers/ai/mcp-server/\n- name: tenantPath\n  type: apiKey\n  in: path\n  name: tenantUUID\n  note: >-\n    Analytics endpoint\
  \ (analytics.planhat.com/analytics/{tenantUUID}) is addressed\n    by tenant UUID in the path; Segment ingest uses Basic auth with tenantUUID as\n    username. Not the main API auth.\n  sources: [https://www.planhat.com/developers/api/user-activities]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planhat/refs/heads/main/authentication/planhat-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Saas
- Customer Success
- Customer Platform
- CRM
- Customer Data
- Analytics
- Revenue
- MCP
---
