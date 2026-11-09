---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 0dteconfluence-com-openapi-generated.yml
  format: yaml
  label: 0DTE Confluence API
  slug: 0dteconfluence-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0dteconfluence-com/openapi/_ae-authored/0dteconfluence-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 0Dteconfluence Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: 0DTE Confluence declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 0DTE Confluence
provider_slug: 0dteconfluence-com
scheme_count: 2
schemes:
- description: API key provided at checkout, used for all /v1/* routes.
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token alternative for API authentication.
  scheme: bearer
  type: http
slug: 0dteconfluence-com-authentication
source_filename: 0dteconfluence-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://0dteconfluence.com/api\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key provided at checkout, used for all /v1/* routes.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token alternative for API authentication.\n"
source_yaml_url: https://artifacts.apis.io/0dteconfluence-com/authentication/0dteconfluence-com-authentication.yml
summary_line: 2 schemes
tags:
- Trading
- Options
- Market Data
- Analytics
- Finance
- Company
---
