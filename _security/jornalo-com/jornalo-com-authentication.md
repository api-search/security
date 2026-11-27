---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Jornalo exposes one machine-facing surface: an MCP server over Streamable HTTP at `https://jornalo.com/api/mcp`. It is protected by OAuth 2.1 and Jornalo is its own authorization server.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jornalo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jornalo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jornalo
provider_slug: jornalo-com
scheme_count: 1
schemes:
- evidence: 'Jornalo exposes one machine-facing surface: an MCP server over Streamable HTTP at `https://jornalo.com/api/mcp`. It is protected by OAuth 2.1 and Jornalo is its own authorization server.'
  flows:
  - authorization_code
  how_to_obtain: Register a client via a client ID metadata document or dynamic client registration, then perform the standard OAuth 2.1 authorization code flow with PKCE.
  name: OAuth 2.1
  scopes:
  - journal:read
  - journal:annotate
  - offline_access
  type: oauth2
slug: jornalo-com-authentication
source_filename: jornalo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://jornalo.com/auth.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://jornalo.com/auth.md\nsources:\n- https://jornalo.com/auth.md\ndescription: 'Jornalo exposes one machine-facing surface: an MCP server over Streamable HTTP at `https://jornalo.com/api/mcp`. It is protected\n  by OAuth 2.1 and Jornalo is its own authorization server.'\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'Jornalo exposes one machine-facing surface: an MCP server over Streamable HTTP at `https://jornalo.com/api/mcp`. It is protected\n    by OAuth 2.1 and Jornalo is its own authorization server.'\n  flows:\n  - authorization_code\n  scopes:\n  - journal:read\n  - journal:annotate\n  - offline_access\n  how_to_obtain: Register a client via a client ID metadata document or dynamic client registration, then perform the standard OAuth 2.1 authorization\n    code flow with PKCE.\ndocs: https://jornalo.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/jornalo-com/authentication/jornalo-com-authentication.yml
summary_line: 1 scheme
tags:
- Trading
- Finance
- Journals
- NinjaTrader
- PropFirms
---
