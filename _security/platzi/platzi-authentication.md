---
api_key_in: []
api_specs:
- filename: platzi-fake-store-openapi-original.json
  format: json
  label: Platzi Fake Store API
  slug: platzi-fake-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platzi/refs/heads/main/openapi/platzi-fake-store-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Platzi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Platzi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Platzi
provider_slug: platzi
scheme_count: 1
schemes:
- bearerFormat: JWT
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - docs
  type: http
slug: platzi-authentication
source_filename: platzi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://fakeapi.platzi.com/en/rest/auth-jwt/\ndocs: https://fakeapi.platzi.com/en/rest/auth-jwt/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  notes: >-\n    The OpenAPI document does not declare a securityScheme, but the API\n    documents JWT bearer authentication. POST /auth/login returns an\n    access_token and refresh_token; the access_token is sent as\n    `Authorization: Bearer <access_token>` on protected endpoints\n    (e.g. GET /auth/profile). Access tokens expire; POST /auth/refresh-token\n    exchanges a refresh_token for a new access_token. Read endpoints\n    (products, categories) are open and require no authentication.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  sources: [docs]\nflows:\n- name: login\n  operation: openapi/platzi-fake-store-openapi-original.json#AuthController_login\n  request:\
  \ 'POST /api/v1/auth/login {email, password}'\n  returns: [access_token, refresh_token]\n- name: refresh\n  operation: openapi/platzi-fake-store-openapi-original.json#AuthController_refreshToken\n  request: 'POST /api/v1/auth/refresh-token {refreshToken}'\n  returns: [access_token, refresh_token]\n- name: profile\n  operation: openapi/platzi-fake-store-openapi-original.json#AuthController_profile\n  request: 'GET /api/v1/auth/profile (Authorization: Bearer <access_token>)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platzi/refs/heads/main/authentication/platzi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Education
- E-Commerce
- Products
- Mock API
- Prototyping
- REST
- GraphQL
- Fake Store
- Developer Tools
---
