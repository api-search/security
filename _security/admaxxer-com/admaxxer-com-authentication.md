---
anonymous_access: false
api_key_in: []
api_specs:
- filename: admaxxer-com-openapi-generated.yml
  format: yaml
  label: Admaxxer API
  slug: admaxxer-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/admaxxer-com/openapi/_ae-authored/admaxxer-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Admaxxer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Admaxxer declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Admaxxer
provider_slug: admaxxer-com
scheme_count: 1
schemes:
- bearerFormat: wk_<token>
  description: API keys are Bearer tokens prefixed with wk_.
  scheme: bearer
  scopes:
  - pixel:read
  - pixel:write
  type: http
slug: admaxxer-com-authentication
source_filename: admaxxer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://admaxxer.com/documentation/api-keys\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: wk_<token>\n    description: API keys are Bearer tokens prefixed with wk_.\n    scopes:\n      - pixel:read\n      - pixel:write\n"
source_yaml_url: https://artifacts.apis.io/admaxxer-com/authentication/admaxxer-com-authentication.yml
summary_line: 1 scheme
tags:
- Analytics
- Attribution
- Artificial Intelligence
- Server-side-tracking
- Ad-ops
- Direct to Consumer
---
