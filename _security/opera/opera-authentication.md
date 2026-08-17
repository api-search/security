---
api_key_in: []
api_specs:
- filename: opera-inventory-api-openapi.yml
  format: yaml
  label: Opera Inventory API
  slug: opera-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-inventory-api-openapi.yml
- filename: opera-marketing-api-openapi.yml
  format: yaml
  label: Opera Marketing API
  slug: opera-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-marketing-api-openapi.yml
- filename: opera-report-api-openapi.yml
  format: yaml
  label: Opera Report API
  slug: opera-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-report-api-openapi.yml
- filename: opera-publisher-report-api-openapi.yml
  format: yaml
  label: Opera Publisher Report API
  slug: opera-publisher-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-publisher-report-api-openapi.yml
- filename: opera-dsp-report-api-openapi.yml
  format: yaml
  label: Opera ADX DSP Report API
  slug: opera-dsp-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-dsp-report-api-openapi.yml
- filename: opera-file-upload-api-openapi.yml
  format: yaml
  label: Opera Ads File Upload API
  slug: opera-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-file-upload-api-openapi.yml
auth_types:
- http
- apiKey
- custom-hmac
- unauthenticated
description: ''
kind: authentication
layout: security
method: searched
name: Opera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opera secures its APIs with http, apiKey, custom-hmac, and unauthenticated across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Opera
provider_slug: opera
scheme_count: 5
schemes:
- description: 'Primary scheme. API token issued by Opera Ads, passed as `Authorization: Bearer <token>`. Used by the advertiser Report API, the publisher Inventory Management API and the publisher OFP Report API.'
  format: Bearer <token>
  header: Authorization
  issuance: Contact Opera Ads (advertiser) or the publisher console (OFP).
  name: bearerAuth
  scheme: bearer
  sources:
  - https://doc.adx.opera.com/advertiser/report-api
  - https://doc.adx.opera.com/publisher/inventory-management-api
  type: http
  used_by:
  - openapi/opera-report-api-openapi.yml
  - openapi/opera-inventory-api-openapi.yml
  - openapi/opera-publisher-report-api-openapi.yml
- description: Legacy exchange reporting. The DSP Report API and the older SSP inventory report take the credential as a `token` QUERY PARAMETER, which puts a long-lived secret into URLs, proxy logs and browser history. Opera's own documentation demonstrates it with a live-looking token in a GET example.
  in: query
  issuance: Issued by Opera to the DSP/SSP partner.
  name: queryToken
  name_param: token
  risk: credential-in-url
  sources:
  - https://doc.adx.opera.com/adx/dsp/report-api
  - https://doc.adx.opera.com/adx/ssp/report
  type: apiKey
  used_by:
  - openapi/opera-dsp-report-api-openapi.yml
  - openapi/opera-publisher-report-api-openapi.yml
- description: File Upload API option A. Static API key issued by the Opera team, prefixed `adx_`. Rotation is by contacting Opera support; there is no self-serve rotation.
  in: header
  key_prefix: adx_
  name: apiKeyAuth
  name_param: X-API-Key
  sources:
  - https://doc.adx.opera.com/advertiser/file_upload_api
  type: apiKey
  used_by:
  - openapi/opera-file-upload-api-openapi.yml
- algorithm: HMAC-SHA256
  description: File Upload API option B and the strongest scheme Opera publishes. Per-request signature over method, path and Unix timestamp; the shared secret never travels with the request, and the timestamp window prevents replay. Opera recommends it over the static API key.
  encoding: lowercase hex
  headers:
  - X-HMAC-Key-Id
  - X-HMAC-Timestamp
  - X-HMAC-Signature
  key_id_prefix: ADX_HMAC_
  name: hmacAuth
  signature_message: '{METHOD}\n{PATH}\n{TIMESTAMP}'
  sources:
  - https://doc.adx.opera.com/advertiser/file_upload_api
  timestamp_window: ±300 seconds
  type: custom-hmac
  used_by:
  - openapi/opera-file-upload-api-openapi.yml
- description: The server-to-server Marketing conversion postback (https://cb.adx.opera.com/marketing/pb) carries NO credential. Identity is the Opera-allocated `cvid` plus the per-click `click_id` captured from the landing-page query string. There is no signature, no shared secret and no timestamp, so the endpoint's integrity rests entirely on click_id secrecy.
  name: none
  sources:
  - https://doc.adx.opera.com/advertiser/events-integration/server-to-server-marketing-api
  type: unauthenticated
  used_by:
  - openapi/opera-marketing-api-openapi.yml
slug: opera-authentication
source_filename: opera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://doc.adx.opera.com/advertiser/report-api +\n  https://doc.adx.opera.com/publisher/inventory-management-api +\n  https://doc.adx.opera.com/publisher/ofp/report +\n  https://doc.adx.opera.com/adx/dsp/report-api +\n  https://doc.adx.opera.com/advertiser/file_upload_api +\n  https://doc.adx.opera.com/advertiser/events-integration/server-to-server-marketing-api\ndocs: https://doc.adx.opera.com/advertiser/report-api\nnote: >-\n  Opera Ads uses FOUR different authentication mechanisms across six APIs, with\n  no single sign-on story and no OAuth anywhere. Every credential is issued by\n  a human at Opera — there is no self-serve key provisioning, no key rotation\n  endpoint, no scopes, and no test/live key distinction. The Marketing\n  conversion postback is unauthenticated: it is identified by an\n  Opera-allocated cvid plus a per-click click_id, which means anyone holding a\n  valid click_id can post an event.\nsummary:\n\
  \  types:\n  - http\n  - apiKey\n  - custom-hmac\n  - unauthenticated\n  oauth2: false\n  openid: false\n  mtls: false\n  self_serve_issuance: false\n  scopes_published: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer <token>'\n  description: >-\n    Primary scheme. API token issued by Opera Ads, passed as\n    `Authorization: Bearer <token>`. Used by the advertiser Report API, the\n    publisher Inventory Management API and the publisher OFP Report API.\n  issuance: Contact Opera Ads (advertiser) or the publisher console (OFP).\n  used_by:\n  - openapi/opera-report-api-openapi.yml\n  - openapi/opera-inventory-api-openapi.yml\n  - openapi/opera-publisher-report-api-openapi.yml\n  sources:\n  - https://doc.adx.opera.com/advertiser/report-api\n  - https://doc.adx.opera.com/publisher/inventory-management-api\n- name: queryToken\n  type: apiKey\n  in: query\n  name_param: token\n  description: >-\n    Legacy exchange reporting.\
  \ The DSP Report API and the older SSP inventory\n    report take the credential as a `token` QUERY PARAMETER, which puts a\n    long-lived secret into URLs, proxy logs and browser history. Opera's own\n    documentation demonstrates it with a live-looking token in a GET example.\n  issuance: Issued by Opera to the DSP/SSP partner.\n  used_by:\n  - openapi/opera-dsp-report-api-openapi.yml\n  - openapi/opera-publisher-report-api-openapi.yml\n  risk: credential-in-url\n  sources:\n  - https://doc.adx.opera.com/adx/dsp/report-api\n  - https://doc.adx.opera.com/adx/ssp/report\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  name_param: X-API-Key\n  key_prefix: adx_\n  description: >-\n    File Upload API option A. Static API key issued by the Opera team, prefixed\n    `adx_`. Rotation is by contacting Opera support; there is no self-serve\n    rotation.\n  used_by:\n  - openapi/opera-file-upload-api-openapi.yml\n  sources:\n  - https://doc.adx.opera.com/advertiser/file_upload_api\n- name:\
  \ hmacAuth\n  type: custom-hmac\n  algorithm: HMAC-SHA256\n  headers:\n  - X-HMAC-Key-Id\n  - X-HMAC-Timestamp\n  - X-HMAC-Signature\n  key_id_prefix: ADX_HMAC_\n  signature_message: '{METHOD}\\n{PATH}\\n{TIMESTAMP}'\n  encoding: lowercase hex\n  timestamp_window: '±300 seconds'\n  description: >-\n    File Upload API option B and the strongest scheme Opera publishes.\n    Per-request signature over method, path and Unix timestamp; the shared\n    secret never travels with the request, and the timestamp window prevents\n    replay. Opera recommends it over the static API key.\n  used_by:\n  - openapi/opera-file-upload-api-openapi.yml\n  sources:\n  - https://doc.adx.opera.com/advertiser/file_upload_api\n- name: none\n  type: unauthenticated\n  description: >-\n    The server-to-server Marketing conversion postback\n    (https://cb.adx.opera.com/marketing/pb) carries NO credential. Identity is\n    the Opera-allocated `cvid` plus the per-click `click_id` captured from the\n    landing-page\
  \ query string. There is no signature, no shared secret and no\n    timestamp, so the endpoint's integrity rests entirely on click_id secrecy.\n  used_by:\n  - openapi/opera-marketing-api-openapi.yml\n  sources:\n  - https://doc.adx.opera.com/advertiser/events-integration/server-to-server-marketing-api\nauthorization:\n  scopes: []\n  note: >-\n    Several APIs return \"403 Forbidden — Insufficient scope\", but Opera\n    publishes no scope registry, no scope names and no way to inspect a token's\n    grants. Nothing derivable; scopes/ is intentionally not written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/authentication/opera-authentication.yml
summary_line: http/apiKey/custom-hmac/unauthenticated · 5 schemes
tags:
- Company
- Consumer Technology
- Advertising
- AdTech
- Browser
- Monetization
- OpenRTB
- Marketing
- Mobile SDK
- Header Bidding
- Publisher Monetization
- Reporting
---
