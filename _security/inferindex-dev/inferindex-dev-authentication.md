---
anonymous_access: true
api_key_in: []
api_specs:
- filename: inferindex-dev-mcp.json
  format: json
  label: InferIndex API
  slug: inferindex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inferindex-dev/openapi/inferindex-dev-mcp.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Inferindex Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: inferindex-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: inferindex-dev
provider_slug: inferindex-dev
scheme_count: 2
schemes:
- description: No authentication required for public read routes.
  type: none
- description: Optional API key to increase rate limits.
  in: header
  name: x-api-key
  type: apiKey
slug: inferindex-dev-authentication
source_filename: inferindex-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://raw.githubusercontent.com/InferIndex/inferindex-docs/main/docs/api.md\nschemes:\n  - type: none\n    description: No authentication required for public read routes.\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: Optional API key to increase rate limits.\n"
source_yaml_url: https://artifacts.apis.io/inferindex-dev/authentication/inferindex-dev-authentication.yml
summary_line: 2 schemes
tags:
- LLM
- Pricing
- Index
- API
- Data
---
