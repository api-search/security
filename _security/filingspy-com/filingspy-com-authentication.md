---
anonymous_access: true
api_key_in: []
auth_types: []
description: Authentication methods for the FilingSpy MCP server.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Filingspy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: FilingSpy declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: FilingSpy
provider_slug: filingspy-com
scheme_count: 3
schemes:
- description: 'Personal MCP API keys look like `fsk_...` and are issued in the FilingSpy Settings > Developer / MCP panel. Supplied to the authenticated endpoint `POST https://filingspy.com/api/mcp` as `Authorization: Bearer YOUR_KEY`. Never print or log the key.'
  evidence: 'Headers: `Authorization: Bearer YOUR_KEY`, `Content-Type: application/json`'
  format: Bearer fsk_...
  header: Authorization
  how_to_obtain: Generate a key in Settings > Developer / MCP at https://filingspy.com/settings
  location: header
  name: FilingSpy API key (Bearer)
  type: http-bearer
- description: OAuth is used by ChatGPT and Claude.ai web connectors. The first connection opens a FilingSpy sign-in page (Google or email link) and a consent screen; no API key is required. Access and rotating refresh tokens can be revoked in Settings > Developer / MCP.
  evidence: '"OAuth connectors (ChatGPT and Claude.ai web) use sign-in with the `mcp` scope: read FilingSpy data as you and share your account''s daily MCP allowance."'
  flow: authorizationCode
  name: FilingSpy OAuth (MCP connectors)
  scopes:
  - mcp
  type: oauth2
- description: Anonymous demo endpoint serves the same tools with no Authorization header, rate-limited to 20 tool calls a day per connection.
  endpoint: https://filingspy.com/api/mcp/demo
  evidence: '"Demo, no account: POST https://filingspy.com/api/mcp/demo serves the same tools with no Authorization header, 20 tool calls a day per connection"'
  name: Anonymous demo endpoint
  type: none
slug: filingspy-com-authentication
source_filename: filingspy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://filingspy.com/SKILL.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local), enriched by docs module\nsource: https://filingspy.com/SKILL.md\nsources:\n- https://filingspy.com/SKILL.md\n- https://filingspy.com/developers/mcp\nname: FilingSpy authentication\ndescription: Authentication methods for the FilingSpy MCP server.\ndocs: https://filingspy.com/developers/mcp\nschemes:\n- type: http-bearer\n  name: FilingSpy API key (Bearer)\n  location: header\n  header: Authorization\n  format: 'Bearer fsk_...'\n  how_to_obtain: Generate a key in Settings > Developer / MCP at https://filingspy.com/settings\n  evidence: 'Headers: `Authorization: Bearer YOUR_KEY`, `Content-Type: application/json`'\n  description: >-\n    Personal MCP API keys look like `fsk_...` and are issued in the FilingSpy\n    Settings > Developer / MCP panel. Supplied to the authenticated endpoint\n    `POST https://filingspy.com/api/mcp` as `Authorization: Bearer YOUR_KEY`.\n    Never print or log the\
  \ key.\n- type: oauth2\n  name: FilingSpy OAuth (MCP connectors)\n  flow: authorizationCode\n  scopes:\n  - mcp\n  evidence: >-\n    \"OAuth connectors (ChatGPT and Claude.ai web) use sign-in with the `mcp`\n    scope: read FilingSpy data as you and share your account's daily MCP\n    allowance.\"\n  description: >-\n    OAuth is used by ChatGPT and Claude.ai web connectors. The first connection\n    opens a FilingSpy sign-in page (Google or email link) and a consent screen;\n    no API key is required. Access and rotating refresh tokens can be revoked\n    in Settings > Developer / MCP.\n- type: none\n  name: Anonymous demo endpoint\n  endpoint: https://filingspy.com/api/mcp/demo\n  evidence: >-\n    \"Demo, no account: POST https://filingspy.com/api/mcp/demo serves the same\n    tools with no Authorization header, 20 tool calls a day per connection\"\n  description: >-\n    Anonymous demo endpoint serves the same tools with no Authorization header,\n    rate-limited to 20 tool calls\
  \ a day per connection.\n"
source_yaml_url: https://artifacts.apis.io/filingspy-com/authentication/filingspy-com-authentication.yml
summary_line: 3 schemes
tags:
- SEC Filings
- 13F
- Insider Trading
- Investor Tracking
- Financial Data
- MCP
- Agents
- Stock Market
---
