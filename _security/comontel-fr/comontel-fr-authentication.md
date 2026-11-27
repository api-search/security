---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Comontel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comontel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Comontel
provider_slug: comontel-fr
scheme_count: 1
schemes:
- applies_to: https://comontel.fr/mcp
  description: The public MCP server requires no authentication. /mcp/info states "authentication":"aucune (données publiques)" and every client connection guide says to connect with no authentication.
  type: none
slug: comontel-fr-authentication
source_filename: comontel-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comontel.fr/mcp/info\ndocs: https://comontel.fr/mcp/info\nschemes:\n- type: none\n  description: The public MCP server requires no authentication. /mcp/info states \"authentication\":\"aucune (données publiques)\" and every client connection guide says to connect with no authentication.\n  applies_to: https://comontel.fr/mcp\nnote: No OpenAPI is published; the only programmatic surface is the read-only MCP server plus static open-data CSV/JSON files at https://comontel.fr/donnees, which are also unauthenticated.\n"
source_yaml_url: https://artifacts.apis.io/comontel-fr/authentication/comontel-fr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Telecommunications
- Mobile
- MVNO
- Cross-Border
- France
- Switzerland
- Small Business
- MCP
---
