---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hooklistener-com-openapi-generated.yml
  format: yaml
  label: Hooklistener API
  slug: hooklistener-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hooklistener-com/openapi/_ae-authored/hooklistener-com-openapi-generated.yml
auth_types: []
description: Authentication methods published by Hooklistener
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Hooklistener Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hooklistener declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Hooklistener
provider_slug: hooklistener-com
scheme_count: 3
schemes:
- evidence: All API requests require authentication using an API key.
  header: Authorization
  how_to_obtain: Create an API key in the dashboard (Organization Settings > API Keys) or via the API using an existing key.
  location: header
  name: API Key
  type: apiKey
- authorize_url: https://app.hooklistener.com/device-codes
  evidence: The CLI uses a secure device code OAuth flow for authentication.
  header: Authorization
  how_to_obtain: Run `hooklistener login` which starts the device code flow, then enter the displayed code at the device‑codes page.
  location: header
  name: Device Code OAuth
  token_url: https://app.hooklistener.com/api/v1/device
  type: http-bearer
- authorize_url: https://app.hooklistener.com/oauth/authorize
  evidence: OAuth 2.0 with discovery metadata, dynamic client registration, and PKCE.
  header: Authorization
  how_to_obtain: Dynamic client registration via POST /oauth/register, then use the authorization code flow (PKCE) to obtain an access token.
  location: header
  name: MCP OAuth
  scopes:
  - full_access
  token_url: https://app.hooklistener.com/oauth/token
  type: http-bearer
slug: hooklistener-com-authentication
source_filename: hooklistener-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.hooklistener.com/guides/build-remote-mcp-server-oauth
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.hooklistener.com/guides/build-remote-mcp-server-oauth\nsources:\n- https://www.hooklistener.com/guides/build-remote-mcp-server-oauth\n- https://www.hooklistener.com/learn/webhook-authentication-strategies\n- https://docs.hooklistener.com/cli/authentication/\n- https://docs.hooklistener.com/api/authentication/\ndescription: Authentication methods published by Hooklistener\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All API requests require authentication using an API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard (Organization Settings > API Keys) or via the API using an existing key.\n- type: http-bearer\n  name: Device Code OAuth\n  evidence: The CLI uses a secure device code OAuth flow for authentication.\n  location: header\n  header: Authorization\n  token_url: https://app.hooklistener.com/api/v1/device\n\
  \  authorize_url: https://app.hooklistener.com/device-codes\n  how_to_obtain: Run `hooklistener login` which starts the device code flow, then enter the displayed code at the device‑codes page.\n- type: http-bearer\n  name: MCP OAuth\n  evidence: OAuth 2.0 with discovery metadata, dynamic client registration, and PKCE.\n  location: header\n  header: Authorization\n  token_url: https://app.hooklistener.com/oauth/token\n  authorize_url: https://app.hooklistener.com/oauth/authorize\n  scopes:\n  - full_access\n  how_to_obtain: Dynamic client registration via POST /oauth/register, then use the authorization code flow (PKCE) to obtain an access token.\ndocs: https://www.hooklistener.com/guides/build-remote-mcp-server-oauth\n"
source_yaml_url: https://artifacts.apis.io/hooklistener-com/authentication/hooklistener-com-authentication.yml
summary_line: 3 schemes
tags:
- Webhook
- Artificial Intelligence
- Debugging
- Developer Tool
- MCP
---
