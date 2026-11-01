---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instapi-co-openapi-generated.yml
  format: yaml
  label: instapi-co API
  slug: instapi-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instapi-co/openapi/_ae-authored/instapi-co-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Instapi Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: instapi-co declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: instapi-co
provider_slug: instapi-co
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Authorization header with Bearer token. Use JWT account token (jwt_instapi_...) for account, key, billing endpoints, or API key token (sk_instapi_...) for Instagram data endpoints.
  scheme: bearer
  type: http
slug: instapi-co-authentication
source_filename: instapi-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://instapi.co/docs\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Authorization header with Bearer token. Use JWT account token (jwt_instapi_...) for account, key, billing endpoints, or API key token (sk_instapi_...) for Instagram data endpoints.\"\n"
source_yaml_url: https://artifacts.apis.io/instapi-co/authentication/instapi-co-authentication.yml
summary_line: 1 scheme
tags:
- Instagram
- Search
- Enrichment
- API
- Social Media
---
