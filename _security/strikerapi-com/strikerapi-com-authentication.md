---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Strikerapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: strikerapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: strikerapi-com
provider_slug: strikerapi-com
scheme_count: 2
schemes:
- description: API key passed in header
  in: header
  name: x-api-key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token API key
  scheme: bearer
  type: http
slug: strikerapi-com-authentication
source_filename: strikerapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://strikerapi.com/docs\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key passed in header\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token API key\n"
source_yaml_url: https://artifacts.apis.io/strikerapi-com/authentication/strikerapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Soccer
- Sports Data
- Odds
- Statistics
- API
---
