---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Feedlio supports two authentication methods: OAuth sign‑in flow and personal access tokens sent as a Bearer token.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Feedlio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feedlio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Feedlio
provider_slug: feedlio-io
scheme_count: 2
schemes:
- evidence: Chat apps sign in with OAuth on feedlio.io; code and scripts use a personal access token.
  header: Authorization
  how_to_obtain: 'Create a token in Settings → MCP → Personal Access Tokens and use it as "Authorization: Bearer fdl_…".'
  location: header
  name: Personal Access Token
  scopes:
  - workspaces:read
  - workspaces:write
  - accounts:read
  - posts:read
  - posts:write
  type: http-bearer
- authorize_url: https://feedlio.io/mcp (sign‑in page opened by client)
  evidence: Chat apps sign in with OAuth on feedlio.io; code and scripts use a personal access token.
  flows:
  - authorization_code
  - client_credentials
  how_to_obtain: Client opens Feedlio's sign‑in page, user clicks Allow, then a token is issued. Clients discover the authorization server via /.well-known/oauth-authorization-server and register dynamically, using PKCE (S256).
  name: OAuth
  scopes:
  - workspaces:read
  - workspaces:write
  - accounts:read
  - posts:read
  - posts:write
  type: oauth2
slug: feedlio-io-authentication
source_filename: feedlio-io-authentication.yml
source_heading: Authentication Profile
source_url: https://feedlio.io/en/developers/authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://feedlio.io/en/developers/authentication\nsources:\n- https://feedlio.io/en/developers/authentication\n- https://feedlio.io/en/developers/quickstart\ndescription: 'Feedlio supports two authentication methods: OAuth sign‑in flow and personal access tokens sent as a Bearer token.'\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: Chat apps sign in with OAuth on feedlio.io; code and scripts use a personal access token.\n  location: header\n  header: Authorization\n  scopes:\n  - workspaces:read\n  - workspaces:write\n  - accounts:read\n  - posts:read\n  - posts:write\n  how_to_obtain: 'Create a token in Settings → MCP → Personal Access Tokens and use it as \"Authorization: Bearer fdl_…\".'\n- type: oauth2\n  name: OAuth\n  evidence: Chat apps sign in with OAuth on feedlio.io; code and scripts use a personal access token.\n  flows:\n  - authorization_code\n\
  \  - client_credentials\n  authorize_url: https://feedlio.io/mcp (sign‑in page opened by client)\n  scopes:\n  - workspaces:read\n  - workspaces:write\n  - accounts:read\n  - posts:read\n  - posts:write\n  how_to_obtain: Client opens Feedlio's sign‑in page, user clicks Allow, then a token is issued. Clients discover the authorization server via\n    /.well-known/oauth-authorization-server and register dynamically, using PKCE (S256).\ndocs: https://feedlio.io/en/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/feedlio-io/authentication/feedlio-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Social Media
- Software-as-a-Service
- Marketing
- Artificial Intelligence
---
