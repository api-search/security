---
anonymous_access: false
api_key_in: []
api_specs:
- filename: live-football-api-com-openapi-generated.yml
  format: yaml
  label: live-football-api-com API
  slug: live-football-api-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/live-football-api-com/openapi/_ae-authored/live-football-api-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Live Football Api Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: live-football-api-com declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: live-football-api-com
provider_slug: live-football-api-com
scheme_count: 3
schemes:
- description: API key passed as query parameter
  in: query
  name: api_key
  type: apiKey
- description: 'Bearer token header (Authorization: Bearer YOUR_KEY)'
  in: header
  name: Authorization
  type: apiKey
- description: OAuth (recommended) for AI assistants via MCP server
  type: oauth2
slug: live-football-api-com-authentication
source_filename: live-football-api-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource:\n  - https://www.live-football-api.com/docs\nschemes:\n  - type: apiKey\n    name: api_key\n    in: query\n    description: API key passed as query parameter\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token header (Authorization: Bearer YOUR_KEY)\"\n  - type: oauth2\n    description: OAuth (recommended) for AI assistants via MCP server\n"
source_yaml_url: https://artifacts.apis.io/live-football-api-com/authentication/live-football-api-com-authentication.yml
summary_line: 3 schemes
tags:
- API
- Sports
- Football
- Real-time
- Data
---
