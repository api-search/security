---
api_key_in: []
auth_types:
- signature
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Gcash Authentication
name_suffix: Authentication
oauth_flows: []
overview: GCash secures its APIs with signature and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GCash
provider_slug: gcash
scheme_count: 3
schemes:
- headers:
  - Client-Id
  - Request-Time
  - Signature
  location: header
  name: RequestSignature
  notes: Every Open API call is signed. The Signature header is a comma-separated key=value string carrying algorithm, keyVersion and the signature value. Keys are bound to the partner Client-Id and generated in the API Portal "Request Credentials" wizard.
  signature:
    algorithms:
    - RSA256
    - ECC224
    default: RSA256
    key_version: keyVersion (defaults to latest key bound to Client-Id)
    request_time_format: ISO 8601, millisecond precision (e.g. 2019-05-28T12:12:12+08:00)
  source: https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/call_api
  type: signature
- flow: authorizationCode
  name: UserAuthorization
  notes: Scopes above are the user-information capability scopes named in the mini-program authorization docs; the full scope reference is partner-gated.
  scopes_documented:
  - USER_INFO
  - USER_LOGIN_ID
  - USER_BASE_INFO
  source: https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/api_openapi_userauthorization
  steps:
  - my.getAuthCode / user authorization consent yields an authCode
  - POST /v{1,2}/authorizations/applyToken exchanges authCode for accessToken
  type: oauth2
- location: partner-portal-issued
  name: PortalCredentials
  notes: Partner applications receive credentials via the GCash API Portal after subscribing to an API product and being approved. Portal login is email-based; production apiportal.gcash.com, sandbox apiportal.lab.gcash.com.
  source: https://gcash.com/business/api-portal-faqs
  type: apiKey
slug: gcash-authentication
source_filename: gcash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/call_api\ndocs:\n- https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/call_api\n- https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/api_openapi_userauthorization\n- https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/v2_applytoken\n- https://gcash.com/business/api-portal-faqs\nsummary:\n  types: [signature, oauth2]\n  model: >-\n    GCash Mini Program Open API uses per-request digital-signature\n    authentication (asymmetric key pair per partner) plus an OAuth2\n    authorization-code style user-authorization flow that mints access tokens\n    for user-scoped operations. The partner API Portal issues client\n    credentials after subscription approval.\nschemes:\n- name: RequestSignature\n  type: signature\n  location: header\n  headers:\n  - Client-Id\n  - Request-Time\n  - Signature\n  signature:\n    algorithms: [RSA256, ECC224]\n    default:\
  \ RSA256\n    key_version: keyVersion (defaults to latest key bound to Client-Id)\n    request_time_format: ISO 8601, millisecond precision (e.g. 2019-05-28T12:12:12+08:00)\n  notes: >-\n    Every Open API call is signed. The Signature header is a comma-separated\n    key=value string carrying algorithm, keyVersion and the signature value.\n    Keys are bound to the partner Client-Id and generated in the API Portal\n    \"Request Credentials\" wizard.\n  source: https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/call_api\n- name: UserAuthorization\n  type: oauth2\n  flow: authorizationCode\n  steps:\n  - my.getAuthCode / user authorization consent yields an authCode\n  - POST /v{1,2}/authorizations/applyToken exchanges authCode for accessToken\n  scopes_documented: [USER_INFO, USER_LOGIN_ID, USER_BASE_INFO]\n  notes: >-\n    Scopes above are the user-information capability scopes named in the\n    mini-program authorization docs; the full scope reference is partner-gated.\n  source:\
  \ https://miniprogram.gcash.com/docs/miniprogram_gcash/mpdev/api_openapi_userauthorization\n- name: PortalCredentials\n  type: apiKey\n  location: partner-portal-issued\n  notes: >-\n    Partner applications receive credentials via the GCash API Portal after\n    subscribing to an API product and being approved. Portal login is\n    email-based; production apiportal.gcash.com, sandbox apiportal.lab.gcash.com.\n  source: https://gcash.com/business/api-portal-faqs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcash/refs/heads/main/authentication/gcash-authentication.yml
summary_line: signature/oauth2 · 3 schemes
tags:
- Company
- Payments
- Mobile Wallet
- E-Money
- Fintech
- Digital Payments
- Philippines
- QR Payments
---
