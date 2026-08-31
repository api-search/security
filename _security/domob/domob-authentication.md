---
api_key_in: []
api_specs:
- filename: domob-reporting-api-openapi.yml
  format: yaml
  label: domob Reporting API
  slug: domob-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domob/refs/heads/main/openapi/domob-reporting-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Domob Authentication
name_suffix: Authentication
oauth_flows: []
overview: domob declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: domob
provider_slug: domob
scheme_count: 3
schemes:
- api: domob-media-data-api
  description: Not a credential. The header value is base64(AES/CBC/PKCS7(slot_id + end_dt + start_dt)) computed with a SHARED SYMMETRIC KEY that Domob prints in the public PDF alongside a worked Golang implementation. Because the key is published, any reader can mint a valid Token, so this header is an integrity/format check rather than authentication.
  in: header
  name: TokenHeader
  parameter: Token
  required: true
  scoped: false
  source: Media Data API PDF, section 2 (加密请求)
  type: apiKey
- api: domob-media-data-api
  description: The developer-platform account email and password, transmitted in the JSON request payload of every call. This is the only real credential on the API. There is no API key, no token issuance step and no way to scope access to reporting only — a leaked value is a full account takeover on the developer platform.
  in: body
  name: AccountCredentialsInBody
  parameter: user_info.username / user_info.password
  required: true
  scoped: false
  source: Media Data API PDF, section 3 (请求参数 / userInfo)
  type: credentials-in-body
- api: domob-reporting-api
  description: Static API token passed as the `key` query-string parameter on every request. Query-string credentials are logged by proxies and servers by default. The API's host (dvx.domob.cn) no longer resolves, so this scheme is documented but not callable.
  in: query
  name: ApiTokenQueryParam
  parameter: key
  required: true
  scoped: false
  source: reporting_api.md, sections 1-3
  status: retired-host
  type: apiKey
slug: domob-authentication
source_filename: domob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://landing.domobcdn.com/2022/adxFile/%E5%AA%92%E4%BD%93%E6%95%B0%E6%8D%AEAPI%E6%8E%A5%E5%8F%A3.pdf\n  (Media Data API, 2024-11-01) and\n  https://github.com/domob-inc/reporting_api/blob/master/reporting_api.md\n  (Reporting API for Publishers v1.0.3), cross-checked against a live\n  unauthenticated probe of https://developer.domob.cn/developer/api/get/stats\ndocs: https://developer.domob.cn/#/doc/api\nsummary: >-\n  Domob publishes no OAuth, no OpenID Connect and no token-exchange flow. Both\n  documented APIs authenticate with long-lived static credentials: the current\n  Media Data API sends the developer-platform account EMAIL AND PASSWORD in the\n  JSON request body on every call, and the legacy Reporting API sends a static\n  API token as a query-string parameter. Neither carries scopes, expiry, or a\n  documented rotation path.\nschemes:\n  - name: TokenHeader\n    api: domob-media-data-api\n    type: apiKey\n\
  \    in: header\n    parameter: Token\n    required: true\n    scoped: false\n    description: >-\n      Not a credential. The header value is base64(AES/CBC/PKCS7(slot_id +\n      end_dt + start_dt)) computed with a SHARED SYMMETRIC KEY that Domob prints\n      in the public PDF alongside a worked Golang implementation. Because the key\n      is published, any reader can mint a valid Token, so this header is an\n      integrity/format check rather than authentication.\n    source: Media Data API PDF, section 2 (加密请求)\n  - name: AccountCredentialsInBody\n    api: domob-media-data-api\n    type: credentials-in-body\n    in: body\n    parameter: user_info.username / user_info.password\n    required: true\n    scoped: false\n    description: >-\n      The developer-platform account email and password, transmitted in the JSON\n      request payload of every call. This is the only real credential on the API.\n      There is no API key, no token issuance step and no way to scope access to\n\
  \      reporting only — a leaked value is a full account takeover on the developer\n      platform.\n    source: Media Data API PDF, section 3 (请求参数 / userInfo)\n  - name: ApiTokenQueryParam\n    api: domob-reporting-api\n    type: apiKey\n    in: query\n    parameter: key\n    required: true\n    scoped: false\n    status: retired-host\n    description: >-\n      Static API token passed as the `key` query-string parameter on every\n      request. Query-string credentials are logged by proxies and servers by\n      default. The API's host (dvx.domob.cn) no longer resolves, so this scheme\n      is documented but not callable.\n    source: reporting_api.md, sections 1-3\nfindings:\n  - id: credentials-in-request-body\n    severity: high\n    detail: >-\n      Account password is a request-payload field on the only live documented\n      API. There is no token layer between the reporting integration and the\n      developer-platform login.\n  - id: shared-signing-key-published\n    severity:\
  \ high\n    detail: >-\n      The AES key used to build the `Token` header is printed verbatim in the\n      provider's own public PDF, so the header cannot authenticate a caller.\n      The key value is deliberately not reproduced in this repository.\n  - id: no-oauth-no-oidc\n    severity: medium\n    detail: >-\n      No oauth2 or openIdConnect scheme is documented on any Domob surface. No\n      /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n      responded with a real document on any host (see well-known/domob-well-known.yml).\n  - id: no-scopes\n    severity: medium\n    detail: >-\n      No permission or scope model is published; access is all-or-nothing per\n      account. Consequently no scopes/ artifact is emitted.\n  - id: no-rotation-policy\n    severity: medium\n    detail: No credential rotation, expiry or revocation policy is documented.\n  - id: plaintext-http-in-legacy-docs\n    severity: medium\n    detail: >-\n      Every worked example\
  \ in reporting_api.md uses http:// (not https://) against\n      dvx.domob.cn, sending the API token in cleartext.\ngated_surfaces:\n  - host: adx.domob.cn\n    status: 401\n    note: >-\n      The Domob ADX endpoint answers HTTP 401 to an anonymous request. Its\n      docking document is on a Feishu wiki that redirects to a BlueFocus SSO\n      login, so its auth scheme could not be read.\n  - host: open.domob.cn\n    status: 200\n    note: >-\n      Self-identifies as \"Domob Open API\" and returns structured error envelopes\n      ({\"error_code\":\"10103\"}), but publishes no discoverable documentation, so\n      no auth scheme could be established.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domob/refs/heads/main/authentication/domob-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Advertising
- Mobile
- AdTech
- Marketing
- SDK
- DSP
- Monetization
- Reporting
- China
---
