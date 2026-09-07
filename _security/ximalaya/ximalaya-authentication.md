---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ximalaya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ximalaya declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Ximalaya
provider_slug: ximalaya
scheme_count: 3
schemes:
- applies_to: all APIs except user-private data APIs
  companion_secret: app_secret
  description: Application public key issued when an app is created in the Open Platform management console. Sent as the `app_key` request parameter alongside the computed `sig`.
  docs: https://open.ximalaya.com/doc/detailApi?categoryId=7&articleId=70
  id: app_key_signature
  in: query_or_form
  name: app_key
  server_side_extra_key: serverAuthStaticKey
  server_side_note: Applications approved for server-side (API) access receive an additional serverAuthStaticKey. For those apps the HMAC key becomes app_secret concatenated with serverAuthenticateStaticKey. Server-side access also requires an IP allowlist configured in the console.
  type: apiKey
- applies_to: user-private data APIs (profile, subscription, cloud play history)
  description: OAuth 2.0 authorization for accessing a Ximalaya user's own data. The access_token is passed as a request parameter (not an Authorization header) and is signed together with the other parameters.
  docs: https://open.ximalaya.com/doc/detailApi?categoryId=9&articleId=5
  flows:
  - authorization_endpoint: https://api.ximalaya.com/oauth2/v2/authorize
    grant_type: authorization_code
    parameters:
    - client_id
    - client_secret
    - redirect_uri
    - code
    - device_id
    - grant_type
    token_endpoint: https://api.ximalaya.com/oauth2/v2/access_token
  - grant_type: client_credentials
    note: used for app-level (non-user) access; the API access guide's own curl example uses this grant.
    token_endpoint: https://api.ximalaya.com/oauth2/v2/access_token
  - grant_type: refresh_token
    parameters:
    - client_id
    - client_secret
    - refresh_token
    - device_id
    - grant_type
    token_endpoint: https://api.ximalaya.com/oauth2/refresh_token
  id: oauth2
  management_endpoints:
  - path: /oauth2/get_token_info
    purpose: introspect an access_token
  - path: /oauth2/revoke_token
    purpose: revoke an access_token
  - path: /oauth2/revoke_refresh_token
    purpose: revoke a refresh_token
  - path: /oauth2/exchange_access_token
    purpose: exchange a third-party account token for a Ximalaya access_token
  token_transport: request parameter `access_token`
  type: oauth2
- applies_to: partners federating their own user accounts into Ximalaya
  description: Partners may bind their own account system to Ximalaya. The partner exposes a token-validation URL that Ximalaya calls (/ximalaya/validate_third_token), and third_uid + third_token are exchanged for a Ximalaya access_token.
  docs: https://open.ximalaya.com/doc/detailApi?categoryId=9&articleId=60
  id: third_party_account_binding
  type: oauth2
slug: ximalaya-authentication
source_filename: ximalaya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://open.ximalaya.com/doc/detailApi?categoryId=6&articleId=67 (参数组成),\n  https://open.ximalaya.com/doc/detailApi?categoryId=6&articleId=69 (签名算法), https://open.ximalaya.com/doc/detailApi?categoryId=7&articleId=75\n  (OAuth2 标准登录授权指南)\nnote: >-\n  Ximalaya publishes no OpenAPI/Swagger document, so this profile was read from the\n  Open Platform documentation rather than derived from securitySchemes. The docs are\n  served by a JS-rendered SPA; the content was read from the portal's own anonymous\n  documentation backend at https://open.ximalaya.com/api-docs/document?id=<id>.\n\nsummary: >-\n  Every Ximalaya Open Platform call is signed. A public app_key identifies the\n  application and a per-request `sig` signature (HMAC-SHA1 over a canonicalized,\n  base64-encoded parameter string, then MD5 of the raw HMAC bytes) authenticates it.\n  APIs that read user-private data additionally require an OAuth 2.0 access_token.\n  There\
  \ is no bearer-only mode and no unsigned public tier.\n\nschemes:\n- id: app_key_signature\n  type: apiKey\n  in: query_or_form\n  name: app_key\n  applies_to: all APIs except user-private data APIs\n  description: >-\n    Application public key issued when an app is created in the Open Platform\n    management console. Sent as the `app_key` request parameter alongside the\n    computed `sig`.\n  companion_secret: app_secret\n  server_side_extra_key: serverAuthStaticKey\n  server_side_note: >-\n    Applications approved for server-side (API) access receive an additional\n    serverAuthStaticKey. For those apps the HMAC key becomes app_secret\n    concatenated with serverAuthenticateStaticKey. Server-side access also\n    requires an IP allowlist configured in the console.\n  docs: https://open.ximalaya.com/doc/detailApi?categoryId=7&articleId=70\n\n- id: oauth2\n  type: oauth2\n  applies_to: user-private data APIs (profile, subscription, cloud play history)\n  description: >-\n    OAuth\
  \ 2.0 authorization for accessing a Ximalaya user's own data. The\n    access_token is passed as a request parameter (not an Authorization header)\n    and is signed together with the other parameters.\n  token_transport: request parameter `access_token`\n  flows:\n  - grant_type: authorization_code\n    authorization_endpoint: https://api.ximalaya.com/oauth2/v2/authorize\n    token_endpoint: https://api.ximalaya.com/oauth2/v2/access_token\n    parameters: [client_id, client_secret, redirect_uri, code, device_id, grant_type]\n  - grant_type: client_credentials\n    token_endpoint: https://api.ximalaya.com/oauth2/v2/access_token\n    note: used for app-level (non-user) access; the API access guide's own curl example\n      uses this grant.\n  - grant_type: refresh_token\n    token_endpoint: https://api.ximalaya.com/oauth2/refresh_token\n    parameters: [client_id, client_secret, refresh_token, device_id, grant_type]\n  management_endpoints:\n  - path: /oauth2/get_token_info\n    purpose:\
  \ introspect an access_token\n  - path: /oauth2/revoke_token\n    purpose: revoke an access_token\n  - path: /oauth2/revoke_refresh_token\n    purpose: revoke a refresh_token\n  - path: /oauth2/exchange_access_token\n    purpose: exchange a third-party account token for a Ximalaya access_token\n  docs: https://open.ximalaya.com/doc/detailApi?categoryId=9&articleId=5\n\n- id: third_party_account_binding\n  type: oauth2\n  applies_to: partners federating their own user accounts into Ximalaya\n  description: >-\n    Partners may bind their own account system to Ximalaya. The partner exposes a\n    token-validation URL that Ximalaya calls (/ximalaya/validate_third_token), and\n    third_uid + third_token are exchanged for a Ximalaya access_token.\n  docs: https://open.ximalaya.com/doc/detailApi?categoryId=9&articleId=60\n\nsignature:\n  algorithm: HMAC-SHA1 + MD5\n  parameter: sig\n  case: lowercase\n  steps:\n  - Sort every request parameter except `sig` by parameter name in lexicographic\
  \ order,\n    using raw (un-URL-encoded) values.\n  - Join the sorted pairs as key1=val1&key2=val2&...\n  - Base64-encode that string using the UTF-8 charset -> base64EncodedStr.\n  - 'Build the HMAC key: app_secret for client (access_token) style access; app_secret\n    concatenated with serverAuthenticateStaticKey for approved server-side API access.'\n  - Compute HMAC-SHA1(base64EncodedStr, key) and keep the RAW BYTE ARRAY (not its hex\n    string) — the docs call this out explicitly as the most common integration error.\n  - MD5 the raw HMAC bytes to produce the 32-character lowercase `sig`.\n  inbound_callbacks_use_a_different_algorithm: true\n  inbound_callback_note: >-\n    The four provider-to-partner push callbacks (/ximalaya/open_push,\n    /ximalaya/notice_pay_album_update, /ximalaya/order_status_notify,\n    /ximalaya/upload_notify) use a separate \"partner-implemented\" signature algorithm\n    that the partner must verify on receipt.\n  docs: https://open.ximalaya.com/doc/detailApi?categoryId=6&articleId=69\n\
  \ncommon_parameters:\n- name: app_key\n  required: true\n  description: Open Platform application public key.\n- name: client_os_type\n  required: true\n  description: '1=iOS, 2=Android, 3=Web, 4=API/Linux (pure server-side), 5=ECOS, 6=mini-program,\n    7=smart speaker, 8=H5 sub-site. Payment APIs accept only 1 or 2.'\n- name: nonce\n  required: true\n  description: Random string, regenerated per request.\n- name: timestamp\n  required: true\n  description: Unix milliseconds. Must be within 1 hour of server time; within 5 minutes\n    for distribution APIs.\n- name: device_id\n  required: true\n  description: Device identifier (OAID preferred on Android, IDFA on iOS). Optional on\n    a few pure server-side endpoints such as /incr/tracks and /incr/albums.\n- name: device_id_type\n  required: true\n  description: One of OAID, OAID_MD5, Android_ID, Android_ID_MD5, IDFA, IDFA_MD5, UUID.\n- name: server_api_version\n  required: true\n  description: 'API version string; currently 1.0.0. Missing\
  \ value returns error 108.'\n- name: sig\n  required: true\n  description: Computed signature over all other parameters.\n- name: access_token\n  required: conditional\n  description: OAuth2 token; required only on user-private data APIs.\n- name: pack_id\n  required: conditional\n  description: Client package name (Android) or Bundle ID (iOS); required on user-private\n    data APIs when client_os_type is 1 or 2.\n\nreplay_protection:\n  mechanism: nonce + timestamp\n  behavior: reject\n  error_code: 225\n  error_string: ximalaya.duplicate invoke with same nonce and timestamp\n  note: >-\n    Reusing the same nonce and timestamp for the same app_key is REJECTED (error 225,\n    and error 301 on the server-side authentication path). This is anti-replay, not\n    idempotency: a retried request must be re-signed with a fresh nonce, so a client\n    cannot safely replay an identical request to recover from a timeout.\n\ntransport:\n  https_required: true\n  methods: [GET, POST]\n  post_content_type:\
  \ application/x-www-form-urlencoded; charset=UTF-8\n  response_content_type: application/json;charset=UTF-8\n\ngaps:\n- No OpenAPI/Swagger document is published, so securitySchemes cannot be machine-read.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration is\n  served on any Ximalaya host (probed 2026-09-04, all 404 or SPA shell).\n- Credentials are issued only after a commercial onboarding review; there is no\n  self-service key issuance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ximalaya/refs/heads/main/authentication/ximalaya-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Audio
- Podcasts
- Audiobooks
- Media
- Content Distribution
- Streaming
- China
- Entertainment
---
