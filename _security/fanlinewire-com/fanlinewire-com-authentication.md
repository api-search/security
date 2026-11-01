---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fanlinewire-com-openapi-generated.yml
  format: yaml
  label: fanlinewire-com API
  slug: fanlinewire-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanlinewire-com/openapi/_ae-authored/fanlinewire-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Fanlinewire Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: fanlinewire-com declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: fanlinewire-com
provider_slug: fanlinewire-com
scheme_count: 3
schemes:
- description: API key header
  in: header
  name: x-api-key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token authentication
  scheme: bearer
  type: http
- description: API key as query parameter
  in: query
  name: key
  type: apiKey
slug: fanlinewire-com-authentication
source_filename: fanlinewire-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://fanlinewire.com/docs\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key header\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token authentication\n  - type: apiKey\n    name: key\n    in: query\n    description: API key as query parameter\n"
source_yaml_url: https://artifacts.apis.io/fanlinewire-com/authentication/fanlinewire-com-authentication.yml
summary_line: 3 schemes
tags:
- Sports
- Betting
- Odds API
- Real-time
- FanDuel
- Data
---
