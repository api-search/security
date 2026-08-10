---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Toutiao Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Toutiao secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Toutiao
provider_slug: toutiao
scheme_count: 1
schemes:
- credentials:
    client_id_param: client_key
    client_secret_param: client_secret
    note: Application credentials (client key / secret, referred to as App ID and App Secret in the Chinese console) are issued only after an application is created and approved in the open-platform console. Approval is documented as a 1-3 business day review.
  flows:
  - authorizationUrl: https://open.snssdk.com/oauth/authorize/
    flow: authorizationCode
    refreshUrl: https://open.snssdk.com/oauth/refresh_token/
    renewRefreshUrl: https://open.snssdk.com/oauth/renew_refresh_token/
    tokenUrl: https://open.snssdk.com/oauth/access_token/
  host: https://open.snssdk.com
  name: ToutiaoOAuth2
  returned_identity:
  - open_id
  - nickname
  - avatar
  sensitive_data:
    caution: Documented by the provider as an approved-permission-only capability; API Evangelist records the published scheme only and holds no credentials.
    decryption: AES; the key is the application clientSecret and the initialization vector is the first 16 bytes of clientSecret, per the published Toutiao/Xigua OAuth documentation.
    field: encrypt_mobile
    permission: mobile_alert
  sources:
  - https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/
  token_lifetimes:
    access_token: 15 days
    refresh_token: 30 days
    source: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/
  type: oauth2
slug: toutiao-authentication
source_filename: toutiao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\ndocs: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\nnote: >-\n  Derived from the provider's published documentation and confirmed by live probes of the\n  API host. Toutiao publishes no OpenAPI, so no securityScheme block exists to derive from\n  mechanically; every field below is either documented by ByteDance on the Douyin Open\n  Platform (the canonical home of the Toutiao/Xigua developer documentation) or observed\n  in a live unauthenticated request to open.snssdk.com.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  token_transport: >-\n    access-token request header (per the Douyin Open Platform userinfo reference, the\n    same convention the Toutiao/Xigua section inherits)\nschemes:\n- name: ToutiaoOAuth2\n  type: oauth2\n  host: https://open.snssdk.com\n\
  \  sources:\n  - https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://open.snssdk.com/oauth/authorize/\n    tokenUrl: https://open.snssdk.com/oauth/access_token/\n    refreshUrl: https://open.snssdk.com/oauth/refresh_token/\n    renewRefreshUrl: https://open.snssdk.com/oauth/renew_refresh_token/\n  credentials:\n    client_id_param: client_key\n    client_secret_param: client_secret\n    note: >-\n      Application credentials (client key / secret, referred to as App ID and App Secret in\n      the Chinese console) are issued only after an application is created and approved in\n      the open-platform console. Approval is documented as a 1-3 business day review.\n  token_lifetimes:\n    access_token: 15 days\n    refresh_token: 30 days\n    source: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\n  returned_identity:\n  - open_id\n\
  \  - nickname\n  - avatar\n  sensitive_data:\n    permission: mobile_alert\n    field: encrypt_mobile\n    decryption: >-\n      AES; the key is the application clientSecret and the initialization vector is the\n      first 16 bytes of clientSecret, per the published Toutiao/Xigua OAuth documentation.\n    caution: >-\n      Documented by the provider as an approved-permission-only capability; API Evangelist\n      records the published scheme only and holds no credentials.\nendpoints_observed:\n  note: >-\n    Live unauthenticated probes on 2026-08-05. A control path (/oauth/nonexistent_zzz9931/)\n    was probed to confirm these are distinct handlers and not a catch-all: the control\n    returns error_code 16, while each endpoint below returns a different parameter-validation\n    error, which is the differential that confirms the endpoint really exists.\n  control:\n    url: https://open.snssdk.com/oauth/nonexistent_zzz9931/\n    http_status: 200\n    error_code: 16\n  endpoints:\n \
  \ - path: /oauth/authorize/\n    http_status: 200\n    error_code: 10005\n    error_description: 缺少参数 (missing parameter)\n  - path: /oauth/access_token/\n    http_status: 200\n    error_code: 10002\n    error_description: 参数错误 (parameter error)\n  - path: /oauth/refresh_token/\n    http_status: 200\n    error_code: 10005\n    error_description: 缺少参数 (missing parameter)\n  - path: /oauth/renew_refresh_token/\n    http_status: 200\n    error_code: 10005\n    error_description: 缺少参数 (missing parameter)\n  - path: /oauth/userinfo/\n    http_status: 200\n    error_code: 10005\n    error_description: 缺少参数 (missing parameter)\n  - path: /oauth/client_token/\n    http_status: 200\n    error_code: 10002\n    error_description: 参数错误 (parameter error)\ngaps:\n- No OpenAPI or other machine-readable description of the OAuth surface is published.\n- >-\n    No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is\n    served on open.snssdk.com (both probed, both 404), so the\
  \ authorization server is not\n    discoverable by RFC 8414 / OIDC Discovery.\n- The full scope list is visible only inside the authenticated open-platform console.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toutiao/refs/heads/main/authentication/toutiao-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- News
- Content
- Media
- Social
- Recommendation
- Publishing
- ByteDance
- China
- OAuth
---
