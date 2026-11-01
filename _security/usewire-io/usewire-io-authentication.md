---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usewire-io-openapi-generated.yml
  format: yaml
  label: usewire-io API
  slug: usewire-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewire-io/openapi/_ae-authored/usewire-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Usewire Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: usewire-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: usewire-io
provider_slug: usewire-io
scheme_count: 2
schemes:
- description: OAuth 2.1 recommended for individual users and agents.
  flows:
    authorizationCode: {}
  type: oauth2
- description: API Keys recommended for headless agents and server-side automation.
  in: header
  name: Authorization
  type: apiKey
slug: usewire-io-authentication
source_filename: usewire-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.usewire.io/mcp/authentication.md\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 recommended for individual users and agents.\n    flows:\n      authorizationCode: {}\n  - type: apiKey\n    description: API Keys recommended for headless agents and server-side automation.\n    in: header\n    name: \"Authorization\"\n"
source_yaml_url: https://artifacts.apis.io/usewire-io/authentication/usewire-io-authentication.yml
summary_line: 2 schemes
tags:
- AI
- MCP
- Collaboration
- Context
- Platform
---
