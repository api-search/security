---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gramclaw-com-api-openapi.json
  format: json
  label: GramClaw Telegram API API
  slug: gramclaw-telegram-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gramclaw-com/openapi/_original/gramclaw-com-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GramClaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: GramClaw declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: GramClaw
provider_slug: gramclaw-com
scheme_count: 2
schemes:
- evidence: 'Authenticate REST: send it as an Authorization: Bearer header.'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys; the full key (gc_live_…) is shown only at creation.
  location: header
  name: API Key (REST)
  type: http-bearer
- evidence: 'MCP: put it in the server URL as the key parameter.'
  how_to_obtain: Create an API key in Settings → API Keys; the full key (gc_live_…) is shown only at creation.
  location: query
  name: API Key (MCP)
  type: apiKey
slug: gramclaw-com-authentication
source_filename: gramclaw-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gramclaw.com/en/help/api-and-mcp
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gramclaw.com/en/help/api-and-mcp\nsources:\n- https://gramclaw.com/en/help/api-and-mcp\n- https://gramclaw.com/en/help/getting-started\nschemes:\n- type: http-bearer\n  name: API Key (REST)\n  evidence: 'Authenticate REST: send it as an Authorization: Bearer header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys; the full key (gc_live_…) is shown only at creation.\n- type: apiKey\n  name: API Key (MCP)\n  evidence: 'MCP: put it in the server URL as the key parameter.'\n  location: query\n  how_to_obtain: Create an API key in Settings → API Keys; the full key (gc_live_…) is shown only at creation.\ndocs: https://gramclaw.com/en/help/api-and-mcp\n"
source_yaml_url: https://artifacts.apis.io/gramclaw-com/authentication/gramclaw-com-authentication.yml
summary_line: 2 schemes
tags:
- Telegram
- Outreach
- Marketing
- Automation
- MCP
---
