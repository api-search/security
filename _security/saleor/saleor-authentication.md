---
api_key_in:
- header
api_specs:
- filename: saleor-openapi.yml
  format: yaml
  label: Saleor GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saleor/refs/heads/main/openapi/saleor-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Saleor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Saleor secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Saleor
provider_slug: saleor
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: User or app JWT issued by Saleor authentication mutations.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/saleor-openapi.yml
  type: http
- description: 'Saleor App auth token, sent as `Authorization: Bearer <token>` and

    scoped to the installed app''s permissions.'
  in: header
  name: appToken
  parameter: Authorization
  sources:
  - openapi/saleor-openapi.yml
  type: apiKey
slug: saleor-authentication
source_filename: saleor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/saleor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: User or app JWT issued by Saleor authentication mutations.\n  sources:\n  - openapi/saleor-openapi.yml\n- name: appToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Saleor App auth token, sent as `Authorization: Bearer <token>` and\n    scoped to the installed app's permissions.\n  sources:\n  - openapi/saleor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saleor/refs/heads/main/authentication/saleor-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Commerce
- Headless
- eCommerce
- GraphQL
- Open Source
- Python
- TypeScript
---
