---
anonymous_access: true
api_key_in: []
api_specs:
- filename: flatin-pt-openapi.json
  format: json
  label: flatin.pt API
  slug: flatinpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flatin-pt/refs/heads/main/openapi/flatin-pt-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Flatin Pt Authentication
name_suffix: Authentication
oauth_flows: []
overview: flatin.pt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: flatin.pt
provider_slug: flatin-pt
scheme_count: 1
schemes:
- description: No credential required. Call https://flatin.pt/api/v1 or connect an MCP client to https://flatin.pt/mcp directly.
  id: anonymous
  type: none
slug: flatin-pt-authentication
source_filename: flatin-pt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: >-\n  openapi/flatin-pt-openapi.json (no securitySchemes), well-known/flatin-pt-api-onboarding.json\n  (authentication.methods: anonymous/none) and the developer docs at\n  https://flatin.pt/en/tools/api-and-data/#rest.\nsummary: >-\n  Keyless public API. There is no authentication of any kind — no API keys, no OAuth, no accounts.\n  Access is anonymous over HTTPS and throttled per client IP address.\nschemes:\n  - id: anonymous\n    type: none\n    description: No credential required. Call https://flatin.pt/api/v1 or connect an MCP client to https://flatin.pt/mcp directly.\naccount_required: false\nagent_policy: allowed\nnotes:\n  - The MCP server at https://flatin.pt/mcp is also anonymous; no OAuth authorization-server or protected-resource metadata is served (both /.well-known probes returned 404).\n  - Every successful JSON answer carries an attribution field that must be displayed next to the numbers (a licence condition,\
  \ not an auth condition).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flatin-pt/refs/heads/main/authentication/flatin-pt-authentication.yml
summary_line: 1 scheme
tags:
- Real Estate
- Property Tax
- Tax
- IMI
- IMT
- Stamp Duty
- Portugal
- Open Data
- Government Data
- Fiscal Data
- MCP
- AI Agents
---
