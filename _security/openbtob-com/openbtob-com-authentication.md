---
anonymous_access: false
api_key_in: []
auth_types: []
description: OpenBtoB uses API keys presented as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OpenBtoB Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenBtoB declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OpenBtoB
provider_slug: openbtob-com
scheme_count: 1
schemes:
- evidence: 'connect to `https://mcp.openbtob.com/mcp` (Streamable HTTP, JSON-RPC 2.0) with the header `Authorization: Bearer <API_KEY>`.'
  header: Authorization
  how_to_obtain: User creates an API key in Settings → MCP API key (format `opb_…`) and provides it to the client.
  location: header
  name: Bearer
  type: http-bearer
slug: openbtob-com-authentication
source_filename: openbtob-com-authentication.yml
source_heading: Authentication Profile
source_url: https://openbtob.com/auth.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://openbtob.com/auth.md\nsources:\n- https://openbtob.com/auth.md\ndescription: OpenBtoB uses API keys presented as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'connect to `https://mcp.openbtob.com/mcp` (Streamable HTTP, JSON-RPC 2.0) with the header `Authorization: Bearer <API_KEY>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: User creates an API key in Settings → MCP API key (format `opb_…`) and provides it to the client.\ndocs: https://openbtob.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/openbtob-com/authentication/openbtob-com-authentication.yml
summary_line: 1 scheme
tags:
- Trade
- Intelligence
- Small Business
- Global
- HS Codes
---
