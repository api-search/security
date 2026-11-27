---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CloudQuell Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudQuell declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CloudQuell
provider_slug: cloudquell-com
scheme_count: 2
schemes:
- client: public (no secret), client id obtained via POST /register (RFC 7591 DCR shim)
  discovery:
  - GET /.well-known/oauth-protected-resource (RFC 9728)
  - GET /.well-known/oauth-authorization-server (RFC 8414)
  docs: https://docs.cloudquell.com/mcp/connect-auth/authentication/
  grant_types:
  - authorization_code
  - refresh_token
  issuer_identification: RFC 9207
  name: oauth2-pkce
  pkce: S256
  resource: https://mcp.cloudquell.com/mcp
  resource_indicator: RFC 8707
  scopes:
  - https://mcp.cloudquell.com/mcp/read
  - https://mcp.cloudquell.com/mcp/admin:write
  - openid
  - email
  - profile
  token_lifetime: access tokens are short-lived (~1 hour); a refresh token keeps the connection alive without re-prompting
  type: oauth2
- capabilities: read scope only; cannot carry admin:write; org-scoped; one active key per person
  docs: https://docs.cloudquell.com/mcp/connect-auth/api-keys/
  format: cak_ prefix followed by a long random string
  header: 'Authorization: Bearer cak_…'
  lifetime: valid for one year from creation; revocable immediately; Regenerate rotates
  name: service-account-key
  plan: paid organizations
  scheme: bearer
  type: http
slug: cloudquell-com-authentication
source_filename: cloudquell-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.cloudquell.com/mcp/connect-auth/authentication/\ndocs: https://docs.cloudquell.com/mcp/connect-auth/authentication/\nsummary: The hosted MCP server at https://mcp.cloudquell.com/mcp is an OAuth 2.1 resource server (Authorization Code + PKCE\n  S256, public client via a Dynamic Client Registration shim, Amazon Cognito identity at auth.cloudquell.com). Headless access\n  uses a read-only cak_ service-account key sent as a bearer token (paid plans). No REST API is published.\nschemes:\n- name: oauth2-pkce\n  type: oauth2\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  client: public (no secret), client id obtained via POST /register (RFC 7591 DCR shim)\n  discovery:\n  - GET /.well-known/oauth-protected-resource (RFC 9728)\n  - GET /.well-known/oauth-authorization-server (RFC 8414)\n  resource: https://mcp.cloudquell.com/mcp\n  resource_indicator: RFC 8707\n  issuer_identification: RFC\
  \ 9207\n  scopes:\n  - https://mcp.cloudquell.com/mcp/read\n  - https://mcp.cloudquell.com/mcp/admin:write\n  - openid\n  - email\n  - profile\n  token_lifetime: access tokens are short-lived (~1 hour); a refresh token keeps the connection alive without re-prompting\n  docs: https://docs.cloudquell.com/mcp/connect-auth/authentication/\n- name: service-account-key\n  type: http\n  scheme: bearer\n  format: cak_ prefix followed by a long random string\n  header: 'Authorization: Bearer cak_…'\n  capabilities: read scope only; cannot carry admin:write; org-scoped; one active key per person\n  lifetime: valid for one year from creation; revocable immediately; Regenerate rotates\n  plan: paid organizations\n  docs: https://docs.cloudquell.com/mcp/connect-auth/api-keys/\ndocs_api_keys: https://docs.cloudquell.com/mcp/connect-auth/api-keys/\n"
source_yaml_url: https://artifacts.apis.io/cloudquell-com/authentication/cloudquell-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- FinOps
- Cloud Cost Management
- AI Cost Management
- Cost Allocation
- Anomaly Detection
- Multi-Cloud
- MCP
---
