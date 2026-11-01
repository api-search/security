---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Wraps Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: wraps-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: wraps-dev
provider_slug: wraps-dev
scheme_count: 2
schemes:
- description: API Key prefixed with `wraps_` for server-to-server and SDK usage.
  example: 'Authorization: Bearer wraps_abcdef123456'
  in: header
  name: Authorization
  type: apiKey
- bearerFormat: JWT
  description: Session token used by dashboard and browser clients.
  example: 'Authorization: Bearer <session_token>'
  scheme: bearer
  type: http
slug: wraps-dev-authentication
source_filename: wraps-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://wraps.dev/docs/reference/api\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: API Key prefixed with `wraps_` for server-to-server and SDK usage.\n    example: \"Authorization: Bearer wraps_abcdef123456\"\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Session token used by dashboard and browser clients.\n    example: \"Authorization: Bearer <session_token>\"\n"
source_yaml_url: https://artifacts.apis.io/wraps-dev/authentication/wraps-dev-authentication.yml
summary_line: 2 schemes
tags:
- Email
- SES
- Infrastructure
- Platform
---
