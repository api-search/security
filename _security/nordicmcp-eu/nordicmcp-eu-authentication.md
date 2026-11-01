---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nordicmcp-eu-openapi-generated.yml
  format: yaml
  label: nordicmcp-eu API
  slug: nordicmcp-eu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordicmcp-eu/openapi/_ae-authored/nordicmcp-eu-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nordicmcp Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: nordicmcp-eu declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: nordicmcp-eu
provider_slug: nordicmcp-eu
scheme_count: 1
schemes:
- description: MCP endpoint token embedded in the URL path (https://nordicmcp.eu/mcp/<integration>/<token>)
  in: path
  name: token
  type: apiKey
slug: nordicmcp-eu-authentication
source_filename: nordicmcp-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://nordicmcp.eu/docs/quota-tokens\nschemes:\n  - type: apiKey\n    name: token\n    in: path\n    description: MCP endpoint token embedded in the URL path (https://nordicmcp.eu/mcp/<integration>/<token>)\n"
source_yaml_url: https://artifacts.apis.io/nordicmcp-eu/authentication/nordicmcp-eu-authentication.yml
summary_line: 1 scheme
tags:
- Company
- MCP
- AI
- Integrations
- Sweden
---
