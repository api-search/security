---
anonymous_access: false
api_key_in: []
api_specs:
- filename: waspytech-com-openapi-generated.yml
  format: yaml
  label: waspytech-com API
  slug: waspytech-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/waspytech-com/openapi/_ae-authored/waspytech-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Waspytech Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: waspytech-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: waspytech-com
provider_slug: waspytech-com
scheme_count: 2
schemes:
- format: wspy_...
  in: header
  name: Authorization
  type: apiKey
- description: JWT signed token for user sessions
  in: header
  name: Authorization
  type: jwt
slug: waspytech-com-authentication
source_filename: waspytech-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.waspytech.com/authentication.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    format: wspy_...\n  - type: jwt\n    name: Authorization\n    in: header\n    description: JWT signed token for user sessions\n"
source_yaml_url: https://artifacts.apis.io/waspytech-com/authentication/waspytech-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- CRM
- WhatsApp
- Messaging
- Software-as-a-Service
---
