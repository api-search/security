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
- filename: snap-render-com-screenshot-api-openapi.yml
  format: yaml
  label: snap-render-com Screenshot API
  slug: snap-render-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-screenshot-api-openapi.yml
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
auth_types: []
description: Authentication methods for SnapRender MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Snap Render Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: snap-render-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: snap-render-com
provider_slug: snap-render-com
scheme_count: 2
schemes:
- evidence: 'Authentication OAuth 2.0 with PKCE (the sign‑in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients) or an API key in the Authorization: Bearer header (CI, scripts, clients without sign‑in)'
  header: Authorization
  how_to_obtain: API keys are available in your dashboard.
  location: header
  name: API Key
  type: http-bearer
- evidence: Authentication OAuth 2.0 with PKCE (the sign‑in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients)
  how_to_obtain: Sign‑in with SnapRender via the OAuth 2.0 PKCE flow.
  name: OAuth 2.0
  type: oauth2
slug: snap-render-com-authentication
source_filename: snap-render-com-authentication.yml
source_heading: Authentication Profile
source_url: https://snap-render.com/claude
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://snap-render.com/claude\nsources:\n- https://snap-render.com/claude\ndescription: Authentication methods for SnapRender MCP\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Authentication OAuth 2.0 with PKCE (the sign‑in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients) or an API\n    key in the Authorization: Bearer header (CI, scripts, clients without sign‑in)'\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are available in your dashboard.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Authentication OAuth 2.0 with PKCE (the sign‑in in claude.ai, Claude Desktop, Claude Code, Cursor and most MCP clients)\n  how_to_obtain: Sign‑in with SnapRender via the OAuth 2.0 PKCE flow.\ndocs: https://snap-render.com/claude\n"
source_yaml_url: https://artifacts.apis.io/snap-render-com/authentication/snap-render-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Screenshot
- Rendering
- Automation
- Cloud
---
