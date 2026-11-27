---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dexi-net-bookmarks-api-openapi.yml
  format: yaml
  label: Dexi Bookmarks API
  slug: dexi-net-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dexi-net/openapi/dexi-net-bookmarks-api-openapi.yml
- filename: dexi-net-publisher-api-openapi.yml
  format: yaml
  label: Dexi Publisher API
  slug: dexi-net-publisher-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dexi-net/openapi/dexi-net-publisher-api-openapi.yml
auth_types: []
description: 'Dexi provides two authentication methods: OAuth 2.1 for MCP connections and personal API tokens used as Bearer tokens.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dexi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dexi declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dexi
provider_slug: dexi-net
scheme_count: 2
schemes:
- authorize_url: https://mcp.dexi.net/authorize
  evidence: MCP clients never handle long-lived secrets. When a client first connects to `https://mcp.dexi.net/mcp`, it registers itself, opens your browser to a Dexi consent page, and receives short-lived tokens after you approve — the standard OAuth 2.1 flow, handled automatically by the client.
  flows:
  - authorization_code
  how_to_obtain: Dynamic client registration via `POST /register` then run the browser‑based consent flow to receive an authorization code and exchange it for access (`dxm_…`) and refresh (`dxr_…`) tokens.
  name: MCP OAuth
  scopes:
  - notes:read
  - notes:write
  - openid
  - email
  - profile
  type: oauth2
- evidence: 'A token authenticates **exactly one endpoint**: [`POST /api/v1/bookmarks/save`](https://docs.dexi.net/api/save-bookmark).'
  header: Authorization
  how_to_obtain: Create a token in Settings → API tokens; the token is a 44‑character string starting with `dxi_` shown once at creation.
  name: Personal API token
  type: http-bearer
slug: dexi-net-authentication
source_filename: dexi-net-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dexi.net/authentication.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dexi.net/authentication.md\nsources:\n- https://docs.dexi.net/authentication.md\n- https://docs.dexi.net/mcp/oauth.md\n- https://docs.dexi.net/quickstart.md\n- https://docs.dexi.net/mcp/getting-started.md\ndescription: 'Dexi provides two authentication methods: OAuth 2.1 for MCP connections and personal API tokens used as Bearer tokens.'\nschemes:\n- type: oauth2\n  name: MCP OAuth\n  evidence: MCP clients never handle long-lived secrets. When a client first connects to `https://mcp.dexi.net/mcp`, it registers itself, opens\n    your browser to a Dexi consent page, and receives short-lived tokens after you approve — the standard OAuth 2.1 flow, handled automatically\n    by the client.\n  flows:\n  - authorization_code\n  authorize_url: https://mcp.dexi.net/authorize\n  scopes:\n  - notes:read\n  - notes:write\n  - openid\n  - email\n  - profile\n  how_to_obtain: Dynamic\
  \ client registration via `POST /register` then run the browser‑based consent flow to receive an authorization code and\n    exchange it for access (`dxm_…`) and refresh (`dxr_…`) tokens.\n- type: http-bearer\n  name: Personal API token\n  evidence: 'A token authenticates **exactly one endpoint**: [`POST /api/v1/bookmarks/save`](https://docs.dexi.net/api/save-bookmark).'\n  header: Authorization\n  how_to_obtain: Create a token in Settings → API tokens; the token is a 44‑character string starting with `dxi_` shown once at creation.\ndocs: https://docs.dexi.net/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/dexi-net/authentication/dexi-net-authentication.yml
summary_line: 2 schemes
tags:
- Knowledge Management
- Personal-Productivity
- Note Taking
- Bookmarking
- RSS-Feeds
---
