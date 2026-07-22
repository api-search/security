---
api_key_in: []
api_specs:
- filename: yoobic-openapi.json
  format: json
  label: YOOBIC Public API
  slug: yoobic-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoobic/refs/heads/main/openapi/yoobic-openapi.json
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Yoobic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yoobic secures its APIs with http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yoobic
provider_slug: yoobic
scheme_count: 2
schemes:
- bearerFormat: JWT
  header: Authorization
  invalidate_endpoint: https://api.yoobic.com/public/api/auth/invalidate_token
  name: bearer-jwt
  sandbox_token_endpoint: https://api-sandbox.yoobic.com/public/api/auth/login
  scheme: bearer
  sources:
  - https://docs.yoobic.com/api.html
  token_endpoint: https://api.yoobic.com/public/api/auth/login
  type: http
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    scopes: 0
    tokenUrl: /
  name: oauth2
  sources:
  - openapi/yoobic-openapi.json
  status: placeholder-in-spec
  type: oauth2
slug: yoobic-authentication
source_filename: yoobic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.yoobic.com/api.html\ndocs: https://docs.yoobic.com/api.html#section-api-access\nsummary:\n  types:\n  - http-bearer\n  primary: JWT bearer token\nnotes: >-\n  The published OpenAPI declares a placeholder `oauth2` securityScheme\n  (authorizationCode flow with empty scopes and \"/\" URLs), but the documented\n  and operative mechanism is a JWT bearer token. Callers obtain a token from the\n  POST /public/api/auth/login endpoint using credentials issued by YOOBIC, then\n  present it as `Authorization: Bearer <jwt>` on every request. Tokens carry an\n  `expires_in`. A companion POST /public/api/auth/invalidate_token endpoint\n  revokes a token. Optional asymmetric RSA-OAEP request encryption is available.\nschemes:\n- name: bearer-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: Authorization\n  token_endpoint: https://api.yoobic.com/public/api/auth/login\n  invalidate_endpoint: https://api.yoobic.com/public/api/auth/invalidate_token\n\
  \  sandbox_token_endpoint: https://api-sandbox.yoobic.com/public/api/auth/login\n  sources:\n  - https://docs.yoobic.com/api.html\n- name: oauth2\n  type: oauth2\n  status: placeholder-in-spec\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n    scopes: 0\n  sources:\n  - openapi/yoobic-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoobic/refs/heads/main/authentication/yoobic-authentication.yml
summary_line: http-bearer · 2 schemes
tags:
- Company
- Retail
- Frontline Operations
- Task Management
- Workforce
- Microlearning
- Employee Experience
- REST
- Webhooks
- SCIM
---
