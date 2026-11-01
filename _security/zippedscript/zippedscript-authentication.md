---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zippedscript-authentication-api-openapi.yml
  format: yaml
  label: ZippedScript Authentication API
  slug: zippedscript-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-authentication-api-openapi.yml
- filename: zippedscript-direct-api-openapi.yml
  format: yaml
  label: ZippedScript Direct API
  slug: zippedscript-direct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-direct-api-openapi.yml
- filename: zippedscript-employment-api-openapi.yml
  format: yaml
  label: ZippedScript Employment API
  slug: zippedscript-employment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-employment-api-openapi.yml
- filename: zippedscript-institution-api-openapi.yml
  format: yaml
  label: ZippedScript Institution API
  slug: zippedscript-institution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-institution-api-openapi.yml
- filename: zippedscript-reference-checks-api-openapi.yml
  format: yaml
  label: ZippedScript Reference Checks API
  slug: zippedscript-reference-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-reference-checks-api-openapi.yml
- filename: zippedscript-user-api-openapi.yml
  format: yaml
  label: ZippedScript User API
  slug: zippedscript-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-user-api-openapi.yml
- filename: zippedscript-verification-api-openapi.yml
  format: yaml
  label: ZippedScript Verification API
  slug: zippedscript-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-verification-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zippedscript Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZippedScript declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ZippedScript
provider_slug: zippedscript
scheme_count: 2
schemes:
- description: Send API key prefixed with 'Token' in the Authorization header.
  in: header
  name: Authorization
  type: apiKey
- bearerFormat: JWT
  description: Send JWT token prefixed with 'Bearer' in the Authorization header.
  scheme: bearer
  type: http
slug: zippedscript-authentication
source_filename: zippedscript-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.zippedscript.com/get_started/\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Send API key prefixed with 'Token' in the Authorization header.\"\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Send JWT token prefixed with 'Bearer' in the Authorization header.\"\n"
source_yaml_url: https://artifacts.apis.io/zippedscript/authentication/zippedscript-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Education
- Verification
- SaaS
- Background-Check
---
