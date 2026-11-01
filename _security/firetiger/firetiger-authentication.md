---
anonymous_access: false
api_key_in: []
api_specs:
- filename: firetiger-openapi-generated.yml
  format: yaml
  label: Firetiger API
  slug: firetiger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firetiger/openapi/_ae-authored/firetiger-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Firetiger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Firetiger declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Firetiger
provider_slug: firetiger
scheme_count: 2
schemes:
- authorizationUrl: <not-provided>
  description: OAuth interactive flow for clients like Claude Desktop, Cursor, and Claude Code.
  flow: authorization_code
  tokenUrl: <not-provided>
  type: oauth2
- description: API key for scripts, created via UI settings.
  in: header
  name: Authorization
  type: apiKey
slug: firetiger-authentication
source_filename: firetiger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.firetiger.com/llms-full.txt\nschemes:\n  - type: oauth2\n    description: OAuth interactive flow for clients like Claude Desktop, Cursor, and Claude Code.\n    flow: authorization_code\n    authorizationUrl: <not-provided>\n    tokenUrl: <not-provided>\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: API key for scripts, created via UI settings.\n"
source_yaml_url: https://artifacts.apis.io/firetiger/authentication/firetiger-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Startup
- Venture-Backed
- Technology
- API
---
