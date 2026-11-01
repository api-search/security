---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods supported by Botoi APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Botoi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: botoi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: botoi-com
provider_slug: botoi-com
scheme_count: 2
schemes:
- authorize_url: https://auth.acme.com/oauth/authorize
  evidence: OAuth 2.1 with PKCE turns your MCP server from a bearer-token honeypot into a scoped, revocable, auditable resource.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Client registers (dynamic registration) and performs PKCE‑enabled authorization code flow to receive an access token.
  location: header
  name: OAuth 2.1 with PKCE
  scopes:
  - tools:read
  - tools:invoke:safe
  - tools:invoke:destructive
  - resources:read
  type: http-bearer
- evidence: 'All API requests require an API key passed in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Obtain the API key from https://api.botoi.com/docs and include it as a Bearer token in the Authorization header.
  location: header
  name: API key
  type: http-bearer
slug: botoi-com-authentication
source_filename: botoi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://botoi.com/blog/mcp-oauth-2-1-pkce-authorization-guide/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://botoi.com/blog/mcp-oauth-2-1-pkce-authorization-guide/\nsources:\n- https://botoi.com/blog/mcp-oauth-2-1-pkce-authorization-guide/\n- https://botoi.com/blog/api-key-vs-jwt-vs-oauth2/\n- https://botoi.com/blog/email-authentication-spf-dmarc-dkim-guide/\n- https://botoi.com/api/signup\ndescription: Authentication methods supported by Botoi APIs\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 with PKCE\n  evidence: OAuth 2.1 with PKCE turns your MCP server from a bearer-token honeypot into a scoped, revocable, auditable resource.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://auth.acme.com/oauth/authorize\n  scopes:\n  - tools:read\n  - tools:invoke:safe\n  - tools:invoke:destructive\n  - resources:read\n  how_to_obtain: Client registers (dynamic registration) and performs PKCE‑enabled authorization code flow to receive\
  \ an access token.\n- type: http-bearer\n  name: API key\n  evidence: 'All API requests require an API key passed in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the API key from https://api.botoi.com/docs and include it as a Bearer token in the Authorization header.\ndocs: https://botoi.com/blog/mcp-oauth-2-1-pkce-authorization-guide/\n"
source_yaml_url: https://artifacts.apis.io/botoi-com/authentication/botoi-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Tools
- Developer
- Free
---
