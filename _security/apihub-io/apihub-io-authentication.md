---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apihub-io-openapi-generated.yml
  format: yaml
  label: APIHub API
  slug: apihub-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apihub-io/openapi/_ae-authored/apihub-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: APIHub Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIHub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: APIHub
provider_slug: apihub-io
scheme_count: 1
schemes:
- description: 'API key prefixed with ''Bearer'' or raw key. Format: ahk_<32 chars>.'
  format: ahk_
  in: header
  name: Authorization
  type: apiKey
slug: apihub-io-authentication
source_filename: apihub-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://apihub.io/docs/agents/api-keys\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"API key prefixed with 'Bearer' or raw key. Format: ahk_<32 chars>.\"\n    format: \"ahk_\"\n"
source_yaml_url: https://artifacts.apis.io/apihub-io/authentication/apihub-io-authentication.yml
summary_line: 1 scheme
tags:
- Marketplace
- MCP
- Artificial Intelligence
- Payments
---
