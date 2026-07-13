---
api_key_in:
- header
api_specs:
- filename: hasura-asyncapi.yml
  format: yaml
  label: Hasura GraphQL API
  slug: hasura-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/asyncapi/hasura-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hasura Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hasura secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hasura
provider_slug: hasura
scheme_count: 2
schemes:
- description: Admin secret configured via HASURA_GRAPHQL_ADMIN_SECRET.
  in: header
  name: adminSecret
  parameter: x-hasura-admin-secret
  sources:
  - openapi/hasura-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT token, when JWT authentication is configured.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hasura-openapi.yml
  type: http
slug: hasura-authentication
source_filename: hasura-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hasura-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: adminSecret\n  type: apiKey\n  in: header\n  parameter: x-hasura-admin-secret\n  description: Admin secret configured via HASURA_GRAPHQL_ADMIN_SECRET.\n  sources:\n  - openapi/hasura-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token, when JWT authentication is configured.\n  sources:\n  - openapi/hasura-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/authentication/hasura-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Access
- GraphQL
---
