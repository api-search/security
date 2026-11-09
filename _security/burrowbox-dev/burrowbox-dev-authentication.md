---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Burrowbox
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Burrowbox Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Burrowbox declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Burrowbox
provider_slug: burrowbox-dev
scheme_count: 2
schemes:
- evidence: Burrowbox uses bearer tokens in the Authorization header.
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: /oauth/authorize
  evidence: MCP clients that support OAuth (Claude, Cursor, VS Code, the MCP SDKs) can connect to https://burrowbox.dev/mcp with no API key.
  how_to_obtain: Dynamic client registration at POST /oauth/register or use a client ID metadata document; then obtain an authorization code via GET /oauth/authorize with PKCE and exchange it for an access token at POST /oauth/token.
  name: MCP OAuth
  scopes:
  - account
  token_url: /oauth/token
  type: oauth2
slug: burrowbox-dev-authentication
source_filename: burrowbox-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://burrowbox.dev/docs/authentication
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://burrowbox.dev/docs/authentication\nsources:\n- https://burrowbox.dev/docs/authentication\n- https://burrowbox.dev/docs/quickstart\ndescription: Authentication schemes for Burrowbox\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Burrowbox uses bearer tokens in the Authorization header.\n  location: header\n  header: Authorization\n- type: oauth2\n  name: MCP OAuth\n  evidence: MCP clients that support OAuth (Claude, Cursor, VS Code, the MCP SDKs) can connect to https://burrowbox.dev/mcp with no API key.\n  token_url: /oauth/token\n  authorize_url: /oauth/authorize\n  scopes:\n  - account\n  how_to_obtain: Dynamic client registration at POST /oauth/register or use a client ID metadata document; then obtain an authorization code via\n    GET /oauth/authorize with PKCE and exchange it for an access token at POST /oauth/token.\ndocs: https://burrowbox.dev/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/burrowbox-dev/authentication/burrowbox-dev-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Linux Desktop
- Persistent Browser
- Credential Vault
- Pay‑per‑minute
- SaaS Platform
---
