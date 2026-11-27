---
anonymous_access: true
api_key_in: []
api_specs:
- filename: algovault-com-openapi-generated.yml
  format: yaml
  label: AlgoVault API
  slug: algovault-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algovault-com/openapi/_ae-authored/algovault-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AlgoVault Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlgoVault declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AlgoVault
provider_slug: algovault-com
scheme_count: 2
schemes:
- description: Bearer token API key for paid plans
  in: header
  name: Authorization
  type: apiKey
- description: Keyless x402 pay-per-call, no authentication required
  type: none
slug: algovault-com-authentication
source_filename: algovault-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://algovault.com/rest-api\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token API key for paid plans\"\n  - type: none\n    description: \"Keyless x402 pay-per-call, no authentication required\"\n"
source_yaml_url: https://artifacts.apis.io/algovault-com/authentication/algovault-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Trading
- Finance
- MCP
- Cryptocurrency
---
