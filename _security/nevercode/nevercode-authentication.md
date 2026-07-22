---
api_key_in:
- header
api_specs:
- filename: nevercode-openapi-original.json
  format: json
  label: Codemagic REST API
  slug: codemagic-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nevercode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nevercode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nevercode
provider_slug: nevercode
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-auth-token
  sources:
  - openapi/nevercode-openapi-original.json
  type: apiKey
slug: nevercode-authentication
source_filename: nevercode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nevercode-openapi-original.json\ndocs: https://docs.codemagic.io/rest-api/overview/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  note: Personal API token sent in the x-auth-token request header; token is managed in Account settings\n    and can be revoked/regenerated.\nschemes:\n- name: api_key\n  type: apiKey\n  sources:\n  - openapi/nevercode-openapi-original.json\n  in: header\n  parameter: x-auth-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/authentication/nevercode-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Continuous Integration
- Continuous Delivery
- CI/CD
- DevOps
- Mobile
- Flutter
- Builds
- App Distribution
- Code Signing
---
