---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Palate MCP is token‑gated; clients authenticate by sending the token in an Authorization: Bearer header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Palate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Palate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Palate
provider_slug: palatemcp-com
scheme_count: 1
schemes:
- evidence: 'Any client that speaks streamable-HTTP MCP connects with your token in an Authorization: Bearer header.'
  header: Authorization
  how_to_obtain: Create a token in the Palate dashboard (Tokens → Create token) and copy the plt_live_ key.
  location: header
  name: Bearer token
  type: http-bearer
slug: palatemcp-com-authentication
source_filename: palatemcp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://palatemcp.com/docs
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://palatemcp.com/docs\nsources:\n- https://palatemcp.com/docs\ndescription: 'Palate MCP is token‑gated; clients authenticate by sending the token in an Authorization: Bearer header.'\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Any client that speaks streamable-HTTP MCP connects with your token in an Authorization: Bearer header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in the Palate dashboard (Tokens → Create token) and copy the plt_live_ key.\nnote: The page also mentions an OAuth flow for ChatGPT, but no token or authorize URLs, nor scopes, are provided, so no OAuth scheme is recorded.\ndocs: https://palatemcp.com/docs\n"
source_yaml_url: https://artifacts.apis.io/palatemcp-com/authentication/palatemcp-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Design
- Website Builder
- MCP
- Design Tokens
---
