---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Atisbo Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: atisbo-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: atisbo-dev
provider_slug: atisbo-dev
scheme_count: 1
schemes:
- bearerFormat: MCP API key (senso_mcp_...)
  description: 'API key sent as Authorization: Bearer <key>'
  scheme: bearer
  scopes:
  - workspace
  - provisioning
  type: http
slug: atisbo-dev-authentication
source_filename: atisbo-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://www.atisbo.dev/auth.md\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"API key sent as Authorization: Bearer <key>\"\n    bearerFormat: \"MCP API key (senso_mcp_...)\"\n    scopes:\n      - workspace\n      - provisioning\n"
source_yaml_url: https://artifacts.apis.io/atisbo-dev/authentication/atisbo-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Product Management
- Evidence
- Decision Support
- AI
---
