---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adona-robot-com-openapi-generated.yml
  format: yaml
  label: adona-robot-com API
  slug: adona-robot-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adona-robot-com/openapi/_ae-authored/adona-robot-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Adona Robot Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: adona-robot-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: adona-robot-com
provider_slug: adona-robot-com
scheme_count: 2
schemes:
- description: Long-lived API key exchanged for a short-lived bearer token.
  in: header
  name: API Key
  type: apiKey
- bearerFormat: JWT
  description: Twelve-hour access token used for all calls.
  scheme: bearer
  type: http
slug: adona-robot-com-authentication
source_filename: adona-robot-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://adona-robot.com/en/reference#authentication\nschemes:\n  - type: apiKey\n    name: API Key\n    in: header\n    description: Long-lived API key exchanged for a short-lived bearer token.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Twelve-hour access token used for all calls.\n"
source_yaml_url: https://artifacts.apis.io/adona-robot-com/authentication/adona-robot-com-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Market-Data
- Forex
- Metals
- API
- Swiss
---
