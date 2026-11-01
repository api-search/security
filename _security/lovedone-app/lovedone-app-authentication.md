---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lovedone-app-content-api-openapi.yml
  format: yaml
  label: lovedone-app Content API
  slug: lovedone-app-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-content-api-openapi.yml
- filename: lovedone-app-discovery-api-openapi.yml
  format: yaml
  label: lovedone-app Discovery API
  slug: lovedone-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-discovery-api-openapi.yml
- filename: lovedone-app-mcp-api-openapi.yml
  format: yaml
  label: lovedone-app MCP API
  slug: lovedone-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-mcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Lovedone App Authentication
name_suffix: Authentication
oauth_flows: []
overview: lovedone-app declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: lovedone-app
provider_slug: lovedone-app
scheme_count: 3
schemes:
- description: Bearer sk-sand-... keys for family or agency surfaces
  in: header
  name: Authorization
  type: apiKey
- description: OAuth 2.1 with PKCE for hosted connectors
  flow: authorizationCode
  pkce: true
  type: oauth2
- description: Session cookies for in-app agents
  scheme: cookie
  type: http
slug: lovedone-app-authentication
source_filename: lovedone-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: \"https://docs.lovedone.app/mcp.html\"\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer sk-sand-... keys for family or agency surfaces\"\n  - type: oauth2\n    flow: authorizationCode\n    pkce: true\n    description: \"OAuth 2.1 with PKCE for hosted connectors\"\n  - type: http\n    scheme: cookie\n    description: \"Session cookies for in-app agents\"\n"
source_yaml_url: https://artifacts.apis.io/lovedone-app/authentication/lovedone-app-authentication.yml
summary_line: 3 schemes
tags:
- Family Care
- Inbox
- Healthcare
- Communication
- Privacy
---
