---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: three.ws API
  slug: main-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/three-ws/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Three Ws Authentication
name_suffix: Authentication
oauth_flows: []
overview: three-ws declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: three-ws
provider_slug: three-ws
scheme_count: 2
schemes:
- description: Bearer token API key, starts with sk_live_
  in: header
  name: Authorization
  type: apiKey
- description: OAuth tokens for MCP clients and CLI, access token lasts one hour
  flow: client_credentials
  type: oauth2
slug: three-ws-authentication
source_filename: three-ws-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://three.ws/docs/api-reference\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token API key, starts with sk_live_\"\n  - type: oauth2\n    flow: client_credentials\n    description: \"OAuth tokens for MCP clients and CLI, access token lasts one hour\"\n"
source_yaml_url: https://artifacts.apis.io/three-ws/authentication/three-ws-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- 3D
- Agents
- Web3
---
