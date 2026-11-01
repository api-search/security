---
anonymous_access: false
api_key_in: []
api_specs:
- filename: supercompress-dev-openapi-generated.yml
  format: yaml
  label: supercompress-dev API
  slug: supercompress-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/supercompress-dev/openapi/_ae-authored/supercompress-dev-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Supercompress Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: supercompress-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: supercompress-dev
provider_slug: supercompress-dev
scheme_count: 2
schemes:
- description: API key provided in X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token in Authorization header.
  scheme: bearer
  type: http
slug: supercompress-dev-authentication
source_filename: supercompress-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.supercompress.dev/api-reference\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key provided in X-API-Key header.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token in Authorization header.\n"
source_yaml_url: https://artifacts.apis.io/supercompress-dev/authentication/supercompress-dev-authentication.yml
summary_line: 2 schemes
tags:
- LLM
- Compression
- API
- Cost-Reduction
- AI
- DeveloperTools
---
