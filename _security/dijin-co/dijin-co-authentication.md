---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dijin Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dijin declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dijin
provider_slug: dijin-co
scheme_count: 1
schemes:
- authorizationUrl: https://dijin.co/oauth/authorize
  authorization_server_metadata: https://dijin.co/.well-known/oauth-authorization-server
  client_registration: Client ID Metadata Documents (preferred) with DCR fallback
  description: OAuth 2.1 with PKCE + RFC 9728 discovery. WWW-Authenticate header on every MCP 401 response points clients at the Protected Resource Metadata. Access tokens SHA-256-hashed at rest; revocation takes effect within one second.
  flow: authorizationCode
  name: oauth2
  pkce: S256 required ("PKCE S256 required for all OAuth flows. code_challenge_method=S256.")
  protected_resource_metadata: https://dijin.co/.well-known/oauth-protected-resource
  scopes_ref: scopes/dijin-co-scopes.yml
  tokenUrl: https://rwxqzunzxwqqwtnjirab.supabase.co/functions/v1/dijin-oauth-token
  type: oauth2
slug: dijin-co-authentication
source_filename: dijin-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dijin.co/docs/connector ; https://dijin.co/en/mcp\ndocs: https://dijin.co/docs/connector\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256 required (\"PKCE S256 required for all OAuth flows. code_challenge_method=S256.\")\n  authorizationUrl: https://dijin.co/oauth/authorize\n  tokenUrl: https://rwxqzunzxwqqwtnjirab.supabase.co/functions/v1/dijin-oauth-token\n  protected_resource_metadata: https://dijin.co/.well-known/oauth-protected-resource\n  authorization_server_metadata: https://dijin.co/.well-known/oauth-authorization-server\n  client_registration: Client ID Metadata Documents (preferred) with DCR fallback\n  scopes_ref: scopes/dijin-co-scopes.yml\n  description: OAuth 2.1 with PKCE + RFC 9728 discovery. WWW-Authenticate header on every MCP 401 response\n    points clients at the Protected Resource Metadata. Access tokens SHA-256-hashed at rest; revocation\n    takes effect within\
  \ one second.\ntoken_lifetime: Magic-link OTP tokens expire ~1 hour after issue.\nnote: Read from docs only; no authentication endpoint was called.\n"
source_yaml_url: https://artifacts.apis.io/dijin-co/authentication/dijin-co-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Agents
- Memory
- MCP
- Personal Data
- Privacy
- OAuth
---
