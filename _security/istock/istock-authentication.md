---
api_key_in:
- header
api_specs:
- filename: swagger
  format: yaml
  label: iStock API (Getty Platform)
  slug: platform
  spec_type: OpenAPI
  url: https://api.gettyimages.com/swagger
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Istock Authentication
name_suffix: Authentication
oauth_flows: []
overview: iStock secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: iStock
provider_slug: istock
scheme_count: 2
schemes:
- description: API key issued through the Getty Images developer program.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/istock-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via /oauth2/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/istock-openapi.yml
  type: http
slug: istock-authentication
source_filename: istock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/istock-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key issued through the Getty Images developer program.\n  sources:\n  - openapi/istock-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via /oauth2/token.\n  sources:\n  - openapi/istock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/authentication/istock-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Stock Media
- Images
- Video
- Illustrations
- Royalty-Free
- Getty
---
