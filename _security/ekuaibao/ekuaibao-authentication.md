---
api_key_in:
- query
auth_types:
- accessToken
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: Ekuaibao Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ekuaibao secures its APIs with accessToken and jwt across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ekuaibao
provider_slug: ekuaibao
scheme_count: 4
schemes:
- credentials:
  - appKey
  - appSecurity
  in: query
  name: getAccessToken (v1)
  parameter: accessToken
  refresh_endpoint: POST /api/openapi/v1/auth/refreshToken
  returns:
  - accessToken
  - refreshToken
  - expireTime
  - corporationId
  sources:
  - https://docs.ekuaibao.com/docs/open-api/getting-started/auth
  token_endpoint: POST https://app.ekuaibao.com/api/openapi/v1/auth/getAccessToken
  ttl_seconds: 7200
  type: token
- credentials:
  - appKey
  - appSecret
  in: query
  name: getAppAccessToken (v1, self-built app)
  parameter: accessToken
  returns:
  - accessToken
  - timeout
  since: 1.25.0
  sources:
  - https://docs.ekuaibao.com/docs/open-api/getting-started/auth-getAppAccessToken
  token_endpoint: POST https://app.ekuaibao.com/api/openapi/v1/auth/getAppAccessToken
  ttl_seconds: 7200
  type: token
- credentials:
  - appKey
  - appSecurity
  in: query
  name: getAccessToken (v3, tenant/platform)
  parameter: accessToken
  returns:
  - accessToken
  - refreshToken
  - expiresTime
  - scope
  scopes:
  - tenant
  - platform
  sources:
  - https://docs.ekuaibao.com/docs/open-api/getting-started/authV3
  token_endpoint: POST https://open.hosecloud.com/auth/openApi/v3/getAccessToken
  token_format: JWT (RS256)
  ttl_seconds: 7200
  type: jwt
- in: query
  name: temp-auth (temporary redirect authorization)
  notes: Temporary authorization used to open Ekuaibao pages from an external system; expireDate up to 604800 seconds, with an optional overdueTokenRedirect.
  parameter: accessToken
  sources:
  - https://docs.ekuaibao.com/docs/open-api/getting-started/temp-auth
  token_endpoint: POST /api/openapi/v1/auth/getAccessToken (with expireDate)
  type: token
slug: ekuaibao-authentication
source_filename: ekuaibao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.ekuaibao.com/docs/open-api/getting-started/auth\ndocs: https://docs.ekuaibao.com/docs/open-api/getting-started/getting-started\nsummary:\n  model: token\n  types:\n  - accessToken\n  - jwt\n  api_key_in:\n  - query\n  oauth2_flows: []\n  notes: >-\n    Proprietary credential-exchange model. An appKey + appSecurity pair (issued in\n    the tenant admin console: 合思 → 合思+ → 开放接口(新) / 自建应用) is exchanged for a\n    short-lived accessToken. The accessToken is then supplied on every subsequent\n    request as the `accessToken` query parameter (not a standard Authorization\n    header, not OAuth2 authorization-code). The address prefix (host) must first be\n    resolved per tenant/platform via GET /api/openapi/v2/location?corpId=.\nschemes:\n- name: getAccessToken (v1)\n  type: token\n  in: query\n  parameter: accessToken\n  token_endpoint: POST https://app.ekuaibao.com/api/openapi/v1/auth/getAccessToken\n  credentials:\n\
  \  - appKey\n  - appSecurity\n  returns:\n  - accessToken\n  - refreshToken\n  - expireTime\n  - corporationId\n  ttl_seconds: 7200\n  refresh_endpoint: POST /api/openapi/v1/auth/refreshToken\n  sources:\n  - https://docs.ekuaibao.com/docs/open-api/getting-started/auth\n- name: getAppAccessToken (v1, self-built app)\n  type: token\n  in: query\n  parameter: accessToken\n  token_endpoint: POST https://app.ekuaibao.com/api/openapi/v1/auth/getAppAccessToken\n  credentials:\n  - appKey\n  - appSecret\n  returns:\n  - accessToken\n  - timeout\n  ttl_seconds: 7200\n  since: 1.25.0\n  sources:\n  - https://docs.ekuaibao.com/docs/open-api/getting-started/auth-getAppAccessToken\n- name: getAccessToken (v3, tenant/platform)\n  type: jwt\n  in: query\n  parameter: accessToken\n  token_endpoint: POST https://open.hosecloud.com/auth/openApi/v3/getAccessToken\n  credentials:\n  - appKey\n  - appSecurity\n  returns:\n  - accessToken\n  - refreshToken\n  - expiresTime\n  - scope\n  token_format: JWT (RS256)\n\
  \  scopes:\n  - tenant\n  - platform\n  ttl_seconds: 7200\n  sources:\n  - https://docs.ekuaibao.com/docs/open-api/getting-started/authV3\n- name: temp-auth (temporary redirect authorization)\n  type: token\n  in: query\n  parameter: accessToken\n  token_endpoint: POST /api/openapi/v1/auth/getAccessToken (with expireDate)\n  notes: >-\n    Temporary authorization used to open Ekuaibao pages from an external system;\n    expireDate up to 604800 seconds, with an optional overdueTokenRedirect.\n  sources:\n  - https://docs.ekuaibao.com/docs/open-api/getting-started/temp-auth\ndeprecated_schemes:\n- name: realms/auth (legacy self-built app auth)\n  endpoint: POST /api/realms/auth\n  superseded_by: getAppAccessToken (v1)\n  sources:\n  - https://docs.ekuaibao.com/docs/open-api/getting-started/platform-auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ekuaibao/refs/heads/main/authentication/ekuaibao-authentication.yml
summary_line: accessToken/jwt · 4 schemes
tags:
- Company
- Enterprise
- Expense Management
- Spend Management
- Travel and Expense
- Reimbursement
- Finance
- Accounting
- Invoicing
- SaaS
- China
---
