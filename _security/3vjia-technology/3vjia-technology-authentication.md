---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 3vjia-technology-open-platform-openapi.yml
  format: yaml
  label: 3vjia Open Platform API
  slug: 3vjia-technology-open-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3vjia-technology/refs/heads/main/openapi/3vjia-technology-open-platform-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: 3Vjia Technology Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: 3vjia Technology secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: 3vjia Technology
provider_slug: 3vjia-technology
scheme_count: 1
schemes:
- applies_to: all 429 documented operations on open-gateway.3vjia.com
  credential_issuance:
    self_serve: false
    steps:
    - Enterprise administrator applies as a developer at https://dev.3vjia.com/manage/my-app/developer
    - Wait for 3vjia approval
    - Register an application at https://dev.3vjia.com/manage/my-app/app-manage
    - Wait for approval; appId/appKey are then issued
  description: OAuth 2.0 client credentials. appId/appKey are issued after developer + application approval at https://dev.3vjia.com/manage/my-app/developer. Token TTL 7200s; re-requesting invalidates the previous token.
  flows:
  - error_response: '{"error": "invalid_client", "error_description": "invalid client_id and client_secret"}'
    flow: clientCredentials
    parameters:
      client_id: the application's appId
      client_secret: the application's appKey
      grant_type: client_credentials
    request_content_type: application/x-www-form-urlencoded
    scopes: 0
    scopes_note: No scopes are defined. The grant is all-or-nothing at the application level; authorisation is enforced by which operations the enterprise's contract enables, not by scope.
    success_response: '{"access_token": "<token>", "expires_in": 7200}'
    tokenUrl: https://graph.3vjia.com/oauth/token
  name: oauth2ClientCredentials
  sources:
  - https://dev.3vjia.com/v1/document?apiId=3a985690d1a94edd924372f8c10187ca
  - openapi/3vjia-technology-open-platform-openapi.yml
  token:
    expiry_signal: code 1700200026 — 凭证已过期，请重新授权 (observed live on graph.3vjia.com, HTTP 200)
    single_token_rule: Only ONE access_token is valid per application at a time — issuing a new one invalidates the previous one. The provider therefore requires an enterprise-wide central token service ("企业需搭建access_token的中控服务"), and warns that independent per-system fetches will conflict. The documentation also recommends exposing a passive refresh endpoint so a caller that observes an expiry can trigger a refresh rather than waiting for the timer.
    ttl_seconds: 7200
  transport:
    current_gateway: https://open-gateway.3vjia.com — the token is presented as the gateway requires; an unauthenticated call returns HTTP 200 with {"code":100100002,"msg":"缺少访问凭证信息"}.
    legacy_gateway: https://open.3vjia.com/<path>?sysCode=external&access_token=<token> — token in the query string
  type: oauth2
slug: 3vjia-technology-authentication
source_filename: 3vjia-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://dev.3vjia.com/v1/document?apiId=3a985690d1a94edd924372f8c10187ca (获取access_token接口),\n  https://dev.3vjia.com/v1/document?apiId=d39aed16895f4f4bb88df99d38f93fb3 (新手指南),\n  the SSO联合单点登录 specification, and live probes of open-gateway.3vjia.com and\n  graph.3vjia.com on 2026-09-05. Baseline derived by 0-working/derive-authentication.py from\n  openapi/3vjia-technology-open-platform-openapi.yml, then upgraded from the documentation.\ndocs: https://dev.3vjia.com/v1/document?apiId=3a985690d1a94edd924372f8c10187ca\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  self_serve: false\n  sandbox: false\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  applies_to: all 429 documented operations on open-gateway.3vjia.com\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://graph.3vjia.com/oauth/token\n    request_content_type: application/x-www-form-urlencoded\n    parameters:\n\
  \      grant_type: client_credentials\n      client_id: the application's appId\n      client_secret: the application's appKey\n    success_response: '{\"access_token\": \"<token>\", \"expires_in\": 7200}'\n    error_response: '{\"error\": \"invalid_client\", \"error_description\": \"invalid client_id and client_secret\"}'\n    scopes: 0\n    scopes_note: >-\n      No scopes are defined. The grant is all-or-nothing at the application level; authorisation is\n      enforced by which operations the enterprise's contract enables, not by scope.\n  token:\n    ttl_seconds: 7200\n    single_token_rule: >-\n      Only ONE access_token is valid per application at a time — issuing a new one invalidates the\n      previous one. The provider therefore requires an enterprise-wide central token service\n      (\"企业需搭建access_token的中控服务\"), and warns that independent per-system fetches will conflict.\n      The documentation also recommends exposing a passive refresh endpoint so a caller that observes\n\
  \      an expiry can trigger a refresh rather than waiting for the timer.\n    expiry_signal: 'code 1700200026 — 凭证已过期，请重新授权 (observed live on graph.3vjia.com, HTTP 200)'\n  transport:\n    current_gateway: >-\n      https://open-gateway.3vjia.com — the token is presented as the gateway requires; an\n      unauthenticated call returns HTTP 200 with {\"code\":100100002,\"msg\":\"缺少访问凭证信息\"}.\n    legacy_gateway: 'https://open.3vjia.com/<path>?sysCode=external&access_token=<token> — token in the query string'\n  credential_issuance:\n    self_serve: false\n    steps:\n    - Enterprise administrator applies as a developer at https://dev.3vjia.com/manage/my-app/developer\n    - Wait for 3vjia approval\n    - Register an application at https://dev.3vjia.com/manage/my-app/app-manage\n    - Wait for approval; appId/appKey are then issued\n  description: >-\n    OAuth 2.0 client credentials. appId/appKey are issued after developer + application approval at\n    https://dev.3vjia.com/manage/my-app/developer.\
  \ Token TTL 7200s; re-requesting invalidates the\n    previous token.\n  sources:\n  - https://dev.3vjia.com/v1/document?apiId=3a985690d1a94edd924372f8c10187ca\n  - openapi/3vjia-technology-open-platform-openapi.yml\nadditional_mechanisms:\n- name: SSO 联合单点登录 (federated single sign-on)\n  type: signed redirect\n  host: https://sso.3vjia.com/JointLogin/Index\n  signature: MD5(userId + appId + time + appKey)\n  timestamp: 10-digit Unix seconds, ±5 minutes tolerance\n  parameters: [userid, appid, time, sign, redirect_uri]\n  binding: >-\n    An external user id is bound to a 3vjia account either in advance via the account-binding\n    operations, or interactively by the designer on first sign-in.\n  note: >-\n    A separate mechanism from the API token, on a separate host, with a separate credential use of\n    appKey. MD5 without a salt or HMAC construction is weak by modern standards; the ±5 minute\n    window is the only replay bound.\n  sources:\n  - https://dev.3vjia.com/v1/document\
  \ (SSO联合单点登录)\n- name: 授权登录授权码 (authorization code for delegated login)\n  type: temporary code\n  operation: commonApiJoinAuthAuthorize\n  ttl: ten minutes (十分钟内有效)\n  note: >-\n    Exchanges an enterprise user id for a short-lived code plus a token expiry, for opening a 3vjia\n    application as a specific user.\n- name: OSS upload signatures\n  type: short-lived object-storage signature\n  operations:\n  - apiV1ModelOssGetUploadToken\n  - apiV1TextureOssGetUploadToken\n  - apiV1LineOssGetUploadToken\n  - apiV1NjvrStsGetSign\n  note: Direct-to-object-storage uploads are authorised by a separately issued, short-lived signature.\ngaps:\n- No scopes, so an application token carries the full contracted surface — no least privilege.\n- No authorization-server metadata (RFC 8414) and no OIDC discovery document.\n- No mutual TLS, no key rotation guidance, no published credential-revocation procedure.\n- No sandbox or test credential; there is nowhere to exercise auth without a production application.\n\
  - Authentication failures return HTTP 200, so standard 401-driven token-refresh middleware will not fire.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3vjia-technology/refs/heads/main/authentication/3vjia-technology-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- 3D Design
- Home Furnishing
- Interior Design
- Manufacturing
- Custom Furniture
- CAD
- Rendering
- Artificial Intelligence
- SaaS
- China
- Open Platform
---
