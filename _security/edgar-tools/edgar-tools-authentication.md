---
anonymous_access: false
api_key_in: []
api_specs:
- filename: edgar-tools-openapi-generated.yml
  format: yaml
  label: edgar.tools API
  slug: edgar-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgar-tools/openapi/_ae-authored/edgar-tools-openapi-generated.yml
auth_types: []
description: Authentication methods for edgar.tools as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: edgar.tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: edgar.tools declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: edgar.tools
provider_slug: edgar-tools
scheme_count: 2
schemes:
- evidence: 'Option 2: X-API-Key header curl -H "X-API-Key: etk_your_key_here" https://api.edgar.tools/v1/search?q=Apple'
  header: X-API-Key
  how_to_obtain: Sign up at edgar.tools/signup, go to Settings → API Keys and click Create API Key. The key is shown once and starts with etk_.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: MCP authentication is handled automatically by your AI client (Claude Desktop, Claude Code, etc.) — when you connect Claude to edgar.tools via MCP, the OAuth flow runs in your browser. Once authorized, your AI client receives a token and uses it transparently for all tool calls.
  header: Authorization
  how_to_obtain: Connect an AI assistant that supports the Model Context Protocol (MCP) to edgar.tools; the assistant will open a browser for sign‑in and issue an OAuth 2.1 token (valid 90 days).
  location: header
  name: MCP OAuth
  type: oauth2
slug: edgar-tools-authentication
source_filename: edgar-tools-authentication.yml
source_heading: Authentication Profile
source_url: https://app.edgar.tools/docs/api/authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.edgar.tools/docs/api/authentication\nsources:\n- https://app.edgar.tools/docs/api/authentication\n- https://app.edgar.tools/docs/quickstart/api\n- https://app.edgar.tools/docs/mcp/setup\ndescription: Authentication methods for edgar.tools as documented\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Option 2: X-API-Key header curl -H \"X-API-Key: etk_your_key_here\" https://api.edgar.tools/v1/search?q=Apple'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Sign up at edgar.tools/signup, go to Settings → API Keys and click Create API Key. The key is shown once and starts with etk_.\n- type: oauth2\n  name: MCP OAuth\n  evidence: MCP authentication is handled automatically by your AI client (Claude Desktop, Claude Code, etc.) — when you connect Claude to edgar.tools\n    via MCP, the OAuth flow runs in your browser. Once authorized, your AI client\
  \ receives a token and uses it transparently for all tool calls.\n  location: header\n  header: Authorization\n  how_to_obtain: Connect an AI assistant that supports the Model Context Protocol (MCP) to edgar.tools; the assistant will open a browser for\n    sign‑in and issue an OAuth 2.1 token (valid 90 days).\ndocs: https://app.edgar.tools/docs/api/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/edgar-tools/authentication/edgar-tools-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Artificial Intelligence
- SEC
- Data
- MCP
---
