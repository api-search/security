---
api_key_in:
- cookie
api_specs:
- filename: blindinsight-openapi-original.yml
  format: yaml
  label: Blind Insight REST API
  slug: blind-insight-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Blindinsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlindInsight secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BlindInsight
provider_slug: blindinsight
scheme_count: 3
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/blindinsight-openapi-original.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/blindinsight-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/blindinsight-openapi-original.yml
  type: http
slug: blindinsight-authentication
source_filename: blindinsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/blindinsight-openapi-original.yml\ndocs: https://docs.blindinsight.io/api-reference/authentication/\nnotes: >-\n  Three authentication methods are documented. JWT Bearer is recommended for\n  production: obtain a token pair via POST /api/token/, send the access token as\n  `Authorization: Bearer <access_token>`, and refresh via POST /api/token/refresh/.\n  HTTP Basic sends `Authorization: Basic <base64(email:password)>` on every request\n  and is the default used by the local Blind Proxy and the blind-ml library.\n  Session/cookie auth uses a `sessionid` cookie after POST /api/accounts/login/,\n  with a CSRF token from GET /api/csrf/. All endpoints require credentials on every\n  request except the public GET /api/status/ health check.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/blindinsight-openapi-original.yml\n\
  - name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/blindinsight-openapi-original.yml\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/blindinsight-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/authentication/blindinsight-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Security
- Encryption
- Privacy
- Confidential Computing
- Data
- Machine Learning
- Compliance
- Cryptography
---
