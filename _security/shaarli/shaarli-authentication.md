---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shaarli-shaarli-api-openapi.yml
  format: yaml
  label: Shaarli API
  slug: shaarli-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shaarli/openapi/shaarli-shaarli-api-openapi.yml
- filename: shaarli-openapi-generated.yml
  format: yaml
  label: Shaarli API
  slug: shaarli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shaarli/openapi/_ae-authored/shaarli-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Shaarli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shaarli declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Shaarli
provider_slug: shaarli
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token must be sent in Authorization header as Bearer token.
  scheme: bearer
  type: http
slug: shaarli-authentication
source_filename: shaarli-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://demo.shaarli.org/doc/html/REST-API.html\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: JWT token must be sent in Authorization header as Bearer token.\n"
source_yaml_url: https://artifacts.apis.io/shaarli/authentication/shaarli-authentication.yml
summary_line: 1 scheme
tags:
- Bookmarking
- Self-hosted
- Open-source
- PHP
- Minimalist
---
