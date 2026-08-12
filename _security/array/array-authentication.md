---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Array Authentication
name_suffix: Authentication
oauth_flows: []
overview: Array secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Array
provider_slug: array
scheme_count: 4
schemes:
- description: Per-application public identifier, a 36-character UUID. Supplied as a query parameter on the embed loader script tag and as an appKey attribute on every array-* web component. The loader rejects any value whose length is not exactly 36. Public by design — it is visible in the page source of every site that embeds an Array component.
  evidence: embed.array.io/cms/array-web-component.js validates appKey length === 36 before init; array.com itself loads the script with ?appKey=<uuid>.
  in: query
  name: appKey
  parameter: appKey
  sources:
  - https://embed.array.io/cms/array-web-component.js
  type: apiKey
- description: Per-consumer user token, sent as a request header from the end user's device. The embed loader sends it on GET https://array.io/api/user/v2 to resolve the userId for the current session. Named for Credmo, the platform Array's credit stack originated from.
  evidence: Observed verbatim in the public loader's inferUserIdFromToken(), which issues fetch('<apiUrl>/api/user/v2') with headers x-credmo-user-token, x-array-web-component-referrer and x-array-web-component.
  in: header
  name: x-credmo-user-token
  parameter: x-credmo-user-token
  sources:
  - https://embed.array.io/cms/array-web-component.js
  type: apiKey
- confidence: medium
  description: Server-side client token, the counterpart to the user token, used when calls are made from the customer's backend rather than the consumer's device. Array's documentation states it must never be placed in website or mobile application source code.
  evidence: Documented by Array on docs.array.com (indexed publicly, page itself password-gated). NOT independently verified against a live response — recorded from the provider's own documentation text rather than a probe.
  in: header
  name: x-credmo-client-token
  parameter: x-credmo-client-token
  sources:
  - https://docs.array.com/docs
  type: apiKey
- description: Short-lived capability tokens returned by the credit-report order call and required to retrieve an assembled report. Both are mandatory query parameters on GET https://array.io/api/report/v2.
  evidence: GET https://array.io/api/report/v2 with no parameters returns HTTP 400 naming both as missing required query parameters.
  in: query
  name: reportKey + displayToken
  parameter: reportKey, displayToken
  sources:
  - https://array.io/api/report/v2
  type: apiKey
slug: array-authentication
source_filename: array-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: https://embed.array.io/cms/array-web-component.js\ndocs: https://docs.array.com/docs\nnotes: >-\n  Array publishes no OpenAPI publicly, so this profile was not derived from a spec. It was\n  read from Array's own public embed loader (embed.array.io/cms/array-web-component.js,\n  HTTP 200) and confirmed against live anonymous responses from https://array.io/api. The\n  full authentication reference lives on docs.array.com, which is password-protected at\n  every path, so scope and token-lifetime detail could not be captured.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: appKey\n  type: apiKey\n  in: query\n  parameter: appKey\n  description: >-\n    Per-application public identifier, a 36-character UUID. Supplied as a query parameter on\n    the embed loader script tag and as an appKey attribute on every\
  \ array-* web component.\n    The loader rejects any value whose length is not exactly 36. Public by design — it is\n    visible in the page source of every site that embeds an Array component.\n  evidence: >-\n    embed.array.io/cms/array-web-component.js validates appKey length === 36 before init;\n    array.com itself loads the script with ?appKey=<uuid>.\n  sources:\n  - https://embed.array.io/cms/array-web-component.js\n- name: x-credmo-user-token\n  type: apiKey\n  in: header\n  parameter: x-credmo-user-token\n  description: >-\n    Per-consumer user token, sent as a request header from the end user's device. The embed\n    loader sends it on GET https://array.io/api/user/v2 to resolve the userId for the\n    current session. Named for Credmo, the platform Array's credit stack originated from.\n  evidence: >-\n    Observed verbatim in the public loader's inferUserIdFromToken(), which issues\n    fetch('<apiUrl>/api/user/v2') with headers x-credmo-user-token,\n    x-array-web-component-referrer\
  \ and x-array-web-component.\n  sources:\n  - https://embed.array.io/cms/array-web-component.js\n- name: x-credmo-client-token\n  type: apiKey\n  in: header\n  parameter: x-credmo-client-token\n  description: >-\n    Server-side client token, the counterpart to the user token, used when calls are made\n    from the customer's backend rather than the consumer's device. Array's documentation\n    states it must never be placed in website or mobile application source code.\n  evidence: >-\n    Documented by Array on docs.array.com (indexed publicly, page itself password-gated).\n    NOT independently verified against a live response — recorded from the provider's own\n    documentation text rather than a probe.\n  confidence: medium\n  sources:\n  - https://docs.array.com/docs\n- name: reportKey + displayToken\n  type: apiKey\n  in: query\n  parameter: reportKey, displayToken\n  description: >-\n    Short-lived capability tokens returned by the credit-report order call and required to\n \
  \   retrieve an assembled report. Both are mandatory query parameters on\n    GET https://array.io/api/report/v2.\n  evidence: >-\n    GET https://array.io/api/report/v2 with no parameters returns HTTP 400 naming both as\n    missing required query parameters.\n  sources:\n  - https://array.io/api/report/v2\ngaps:\n- No OAuth 2.0 or OpenID Connect surface is advertised; /.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server return 404 on every Array host.\n- No published token lifetime, rotation, or revocation policy is publicly reachable.\n- No scope or permission model is publicly documented, so no scopes/ artifact is emitted.\nx-evidence:\n- fetched: '2026-08-10'\n  url: https://embed.array.io/cms/array-web-component.js\n  http_status: 200\n- fetched: '2026-08-10'\n  url: https://array.io/api/report/v2\n  http_status: 400\n- fetched: '2026-08-10'\n  url: https://array.io/.well-known/openid-configuration\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/array/refs/heads/main/authentication/array-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Fintech
- Embedded Finance
- Credit Data
- Identity
- Background Checks
- Credit Monitoring
- Consumer Data
- Financial Services
- API
---
