---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kawaa Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: kawaa-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: kawaa-com
provider_slug: kawaa-com
scheme_count: 2
schemes:
- description: API key for authentication.
  in: header
  name: X-Api-Key
  type: apiKey
- bearerFormat: ev_
  description: OAuth short-lived access token.
  scheme: bearer
  type: http
slug: kawaa-com-authentication
source_filename: kawaa-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://kawaa.com/docs/authentication\nschemes:\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: API key for authentication.\n  - type: http\n    scheme: bearer\n    bearerFormat: ev_\n    description: OAuth short-lived access token.\n"
source_yaml_url: https://artifacts.apis.io/kawaa-com/authentication/kawaa-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- EmailVerification
- API
- SaaS
- Marketing
---
