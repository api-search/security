---
api_key_in:
- header
api_specs:
- filename: select-star-openapi.yml
  format: yaml
  label: Select Star Metadata API
  slug: select-star-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/select-star/refs/heads/main/openapi/select-star-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Select Star Authentication
name_suffix: Authentication
oauth_flows: []
overview: Select Star secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Select Star
provider_slug: select-star
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: JWTAuthentication
  scheme: bearer
  sources:
  - openapi/select-star-openapi.yml
  type: http
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/select-star-openapi.yml
  type: apiKey
slug: select-star-authentication
source_filename: select-star-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/select-star-openapi.yml\ndocs: https://docs.selectstar.com/select-star-api/authentication\nnotes: >-\n  REST requests use the header \"Authorization: Token <token>\" — the keyword must\n  be Token, not Bearer. Tokens are created under Account Settings > Client API\n  Token > Manage API Tokens and have no expiration (delete/recreate to rotate).\n  A JWT bearer scheme also exists (used by the hosted MCP server as\n  \"Authorization: Bearer <token>\").\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: JWTAuthentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/select-star-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/select-star-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/select-star/refs/heads/main/authentication/select-star-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Data Catalog
- Data Lineage
- Metadata
- Data Governance
- Semantic Layer
- MCP
- AI-Ready Data
- Analytics
---
