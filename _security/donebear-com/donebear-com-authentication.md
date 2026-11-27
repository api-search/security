---
anonymous_access: false
api_key_in: []
api_specs:
- filename: donebear-com-api-openapi.json
  format: json
  label: Done Bear API API
  slug: done-bear-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/donebear-com/openapi/_original/donebear-com-api-openapi.json
auth_types: []
description: Done Bear API authentication supports bearer tokens (API keys or JWTs) sent in the Authorization header and OAuth2 authorization code flow with PKCE.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Done Bear Authentication
name_suffix: Authentication
oauth_flows: []
overview: Done Bear declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Done Bear
provider_slug: donebear-com
scheme_count: 1
schemes:
- authorize_url: https://mcp.donebear.com/authorize
  evidence: MCP client or other OAuth public client → authorization code + PKCE S256 against https://mcp.donebear.com.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Create a client ID (metadata document or dynamic registration) and perform the OAuth authorization‑code with PKCE flow to receive an access token from https://mcp.donebear.com/token.
  location: header
  name: MCP OAuth
  scopes:
  - read
  - write
  - admin
  type: oauth2
slug: donebear-com-authentication
source_filename: donebear-com-authentication.yml
source_heading: Authentication Profile
source_url: https://donebear.com/docs/api/authentication.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://donebear.com/docs/api/authentication.md\nsources:\n- https://donebear.com/docs/api/authentication.md\n- https://donebear.com/docs/api/authentication\n- https://donebear.com/docs/cli/automation.md\n- https://donebear.com/auth.md\ndescription: Done Bear API authentication supports bearer tokens (API keys or JWTs) sent in the Authorization header and OAuth2 authorization\n  code flow with PKCE.\nschemes:\n- type: oauth2\n  name: MCP OAuth\n  evidence: MCP client or other OAuth public client → authorization code + PKCE S256 against https://mcp.donebear.com.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://mcp.donebear.com/authorize\n  scopes:\n  - read\n  - write\n  - admin\n  how_to_obtain: Create a client ID (metadata document or dynamic registration) and perform the OAuth authorization‑code with PKCE flow to receive\n\
  \    an access token from https://mcp.donebear.com/token.\nnote: API keys are long‑lived db_ keys created via the CLI (`donebear api-key create`) and are sent as Bearer tokens. Supabase JWTs are also accepted\n  as Bearer tokens. 1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://donebear.com/docs/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/donebear-com/authentication/donebear-com-authentication.yml
summary_line: 1 scheme
tags:
- Task Management
- Productivity
- Cross-Platform
- To-Do
- Local-First
---
