---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Callejear.de Authentication
name_suffix: Authentication
oauth_flows: []
overview: Callejear.de declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Callejear.de
provider_slug: callejear-de
scheme_count: 1
schemes:
- description: Public, read-only MCP endpoint; no account or API key. Docs state "Kein API-Schlüssel erforderlich." The GitHub README states "Streamable HTTP, no account or API key".
  evidence:
  - https://callejear.de/mcp/
  - https://github.com/Habanacasta88/callejear-de-mcp
  type: none
slug: callejear-de-authentication
source_filename: callejear-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://callejear.de/mcp/\ndocs: https://callejear.de/mcp/\nschemes:\n- type: none\n  description: Public, read-only MCP endpoint; no account or API key. Docs state \"Kein API-Schlüssel erforderlich.\" The GitHub README states \"Streamable HTTP, no account or API key\".\n  evidence:\n  - https://callejear.de/mcp/\n  - https://github.com/Habanacasta88/callejear-de-mcp\nnote: No OpenAPI or securitySchemes are published; the only surface is the keyless remote MCP server at https://callejear.de/api/mcp.\n"
source_yaml_url: https://artifacts.apis.io/callejear-de/authentication/callejear-de-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Geospatial
- Open Data
- Germany
- Streets
- Real Estate
- MCP
- Location Data
---
