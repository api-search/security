---
anonymous_access: false
api_key_in: []
api_specs:
- filename: archgraph-dev-openapi-generated.yml
  format: yaml
  label: ArchGraph API
  slug: archgraph-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/archgraph-dev/openapi/_ae-authored/archgraph-dev-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ArchGraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: ArchGraph declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ArchGraph
provider_slug: archgraph-dev
scheme_count: 2
schemes:
- description: Bearer token (API Key)
  in: header
  name: Authorization
  type: apiKey
- bearerFormat: JWT
  description: Clerk JWT for web dashboard sessions
  scheme: bearer
  type: http
slug: archgraph-dev-authentication
source_filename: archgraph-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://docs.archgraph.dev/api-reference\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token (API Key)\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Clerk JWT for web dashboard sessions\n"
source_yaml_url: https://artifacts.apis.io/archgraph-dev/authentication/archgraph-dev-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Code Intelligence
- MCP
- Developer Tools
- Platform
---
