---
anonymous_access: false
api_key_in: []
api_specs:
- filename: relaygpu-com-openapi-generated.yml
  format: yaml
  label: relaygpu-com API
  slug: relaygpu-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/relaygpu-com/openapi/_ae-authored/relaygpu-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Relaygpu Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: relaygpu-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: relaygpu-com
provider_slug: relaygpu-com
scheme_count: 2
schemes:
- description: API key for inference endpoints (format relay_sk_...)
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Dashboard JWT for account and key management
  scheme: bearer
  type: http
slug: relaygpu-com-authentication
source_filename: relaygpu-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://opengpu-network.gitbook.io/relay/introduction/authentication.md\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key for inference endpoints (format relay_sk_...)\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Dashboard JWT for account and key management\n"
source_yaml_url: https://artifacts.apis.io/relaygpu-com/authentication/relaygpu-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Compute
- GPU
- Cloud
- API
---
