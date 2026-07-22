---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Weav Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weav secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weav
provider_slug: weav
scheme_count: 1
schemes:
- description: 'Bearer token passed in the Authorization header for all REST calls (Authorization: Bearer <auth_token>). Tokens are environment/workspace scoped; the SDK Config takes an auth_token (SecretStr) plus an env host.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://github.com/weav-ai/weavai-developer-library
  type: http
slug: weav-authentication
source_filename: weav-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/weav-ai/weavai-developer-library\ndocs: https://weav-ai.github.io/\nnotes: >-\n  Derived from the first-party weavaidev Python library source (no public\n  OpenAPI is published). Every service client sends\n  `Authorization: Bearer <auth_token>` with `Accept: application/json`. The\n  token is supplied as a workspace/environment secret (SecretStr auth_token)\n  alongside an `env` value that selects the tenant service host.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token passed in the Authorization header for all REST calls\n    (Authorization: Bearer <auth_token>). Tokens are environment/workspace\n    scoped; the SDK Config takes an auth_token (SecretStr) plus an env host.\n  sources:\n  - https://github.com/weav-ai/weavai-developer-library\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weav/refs/heads/main/authentication/weav-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Insurance
- Insurtech
- Underwriting
- Premium Audit
- Claims
- Document AI
- Property and Casualty
- Decisioning
---
