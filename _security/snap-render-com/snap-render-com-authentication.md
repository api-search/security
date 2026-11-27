---
anonymous_access: false
api_key_in: []
api_specs:
- filename: snap-render-com-extract-api-openapi.yml
  format: yaml
  label: snap-render-com Extract API
  slug: snap-render-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-extract-api-openapi.yml
- filename: snap-render-com-health-api-openapi.yml
  format: yaml
  label: snap-render-com Health API
  slug: snap-render-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-health-api-openapi.yml
- filename: snap-render-com-schedules-api-openapi.yml
  format: yaml
  label: snap-render-com Schedules API
  slug: snap-render-com-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-schedules-api-openapi.yml
- filename: snap-render-com-usage-api-openapi.yml
  format: yaml
  label: snap-render-com Usage API
  slug: snap-render-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-usage-api-openapi.yml
- filename: snap-render-com-webhooks-api-openapi.yml
  format: yaml
  label: snap-render-com Webhooks API
  slug: snap-render-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-webhooks-api-openapi.yml
- filename: snap-render-com-screenshot-api-openapi.yml
  format: yaml
  label: SnapRender Screenshot API
  slug: snap-render-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-screenshot-api-openapi.yml
auth_types: []
description: Authentication methods for SnapRender as published on the page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: SnapRender Authentication
name_suffix: Authentication
oauth_flows: []
overview: SnapRender declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SnapRender
provider_slug: snap-render-com
scheme_count: 2
schemes:
- evidence: 'Authentication OAuth 2.0 with PKCE (the sign-in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients) or an API key in the Authorization: Bearer header (CI, scripts, clients without sign-in)'
  flows:
  - authorization_code
  how_to_obtain: Sign in via the SnapRender sign‑in window that Claude opens and approve the connection.
  name: OAuth 2.0 with PKCE
  type: oauth2
- evidence: 'Authentication OAuth 2.0 with PKCE (the sign-in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients) or an API key in the Authorization: Bearer header (CI, scripts, clients without sign-in)'
  header: 'Authorization: Bearer'
  how_to_obtain: Generate a key in your SnapRender dashboard and use it as the Bearer token.
  location: header
  name: API key
  type: apiKey
slug: snap-render-com-authentication
source_filename: snap-render-com-authentication.yml
source_heading: Authentication Profile
source_url: https://snap-render.com/claude
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://snap-render.com/claude\nsources:\n- https://snap-render.com/claude\ndescription: Authentication methods for SnapRender as published on the page.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 with PKCE\n  evidence: 'Authentication OAuth 2.0 with PKCE (the sign-in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients) or an API\n    key in the Authorization: Bearer header (CI, scripts, clients without sign-in)'\n  flows:\n  - authorization_code\n  how_to_obtain: Sign in via the SnapRender sign‑in window that Claude opens and approve the connection.\n- type: apiKey\n  name: API key\n  evidence: 'Authentication OAuth 2.0 with PKCE (the sign-in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients) or an API\n    key in the Authorization: Bearer header (CI, scripts, clients without sign-in)'\n  location: header\n  header: 'Authorization: Bearer'\n\
  \  how_to_obtain: Generate a key in your SnapRender dashboard and use it as the Bearer token.\ndocs: https://snap-render.com/claude\n"
source_yaml_url: https://artifacts.apis.io/snap-render-com/authentication/snap-render-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Screenshots
- Rendering
- Automation
- Cloud
---
