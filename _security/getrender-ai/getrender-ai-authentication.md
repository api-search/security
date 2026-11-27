---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for GetRender
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GetRender Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetRender declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GetRender
provider_slug: getrender-ai
scheme_count: 1
schemes:
- evidence: The MCP server authenticates with a Bearer token.
  header: Authorization
  how_to_obtain: Create a personal API key in Settings → Connected apps & API keys, or obtain an OAuth access token via the browser flow.
  location: header
  name: Bearer token
  type: http-bearer
slug: getrender-ai-authentication
source_filename: getrender-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://getrender.ai/docs/reference/authentication
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getrender.ai/docs/reference/authentication\nsources:\n- https://getrender.ai/docs/reference/authentication\n- https://getrender.ai/docs/getting-started/mcp-quickstart\n- https://getrender.ai/docs/getting-started/overview\n- https://getrender.ai/docs/getting-started/web-quickstart\ndescription: Authentication schemes for GetRender\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: The MCP server authenticates with a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal API key in Settings → Connected apps & API keys, or obtain an OAuth access token via the browser flow.\ndocs: https://getrender.ai/docs/reference/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/getrender-ai/authentication/getrender-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Rendering
- Architecture
- Design
---
