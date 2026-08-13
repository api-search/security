---
api_key_in:
- body
auth_types:
- none
- custom-credential-pair
description: ''
kind: authentication
layout: security
method: probed
name: Minute Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Minute Media secures its APIs with none and custom-credential-pair across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Minute Media
provider_slug: minute-media
scheme_count: 2
schemes:
- api: STN Video oEmbed API
  base_url: https://embed.sendtonews.com/services/oembed
  description: The oEmbed 1.0 endpoint is public and unauthenticated. A GET with a `url` parameter naming an embed.sendtonews.com resource returns a 200 oEmbed video payload with no credential of any kind.
  evidence:
  - content_type: application/json; charset=UTF-8
    observed: '2026-08-12'
    request: GET https://embed.sendtonews.com/services/oembed?url=https%3A%2F%2Fembed.sendtonews.com%2Foembed%2F%3FSC%3D<share-code>&format=json
    status: 200
  name: none
  type: none
- api: STN Video Publisher API
  base_url: https://api.sendtonews.com/api/v1/
  description: Every STN Video Publisher API operation carries the same credential pair in the POST body — there is no header scheme, no bearer token, no OAuth, and no scope model. The plugin additionally sends non-credential telemetry fields (appName, appVersion, cmsVersion, appComponent) on the verification call.
  evidence:
  - observed: '2026-08-12'
    request: POST https://api.sendtonews.com/api/v1/auth/verifycode (no body)
    response: '{"success":false,"code":422,"errors":{"authcode":"authcode is required","cid":"cid is required"}}'
    status: 422
  - observed: '2026-08-12'
    request: POST https://api.sendtonews.com/api/v1/players (no body)
    response: '{"success":false,"code":422,"errors":{"authcode":"authcode is required","cid":"cid is required"}}'
    status: 422
  - kind: first-party client source
    source: sendtonews/app/Controllers/AdminController.php (plugin v1.2.2)
  in: body
  issuance: Credentials are not self-serve. The publisher documentation directs integrators to publishers@stnvideo.com to obtain a Company ID and Authentication Code, so the API is customer-gated rather than open.
  name: cid + authcode
  parameters:
  - description: Company ID issued by STN Video to a publisher account.
    name: cid
  - description: Authentication Code issued alongside the Company ID.
    name: authcode
  transport: POST, application/x-www-form-urlencoded request body
  type: custom-credential-pair
  verification_operation: POST /api/v1/auth/verifycode
slug: minute-media-authentication
source_filename: minute-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  First-party STN Video WordPress Player Selector plugin source\n  (https://www.stnvideo.com/wp-plugin/sendtonews.zip, v1.2.2) plus live unauthenticated\n  requests to https://api.sendtonews.com/api/v1/ and\n  https://embed.sendtonews.com/services/oembed on 2026-08-12.\ndocs: https://www.stnvideo.com/resources/our-wordpress-ovp-plugin/\nnotes: >-\n  Minute Media publishes no OpenAPI and no API reference, so this profile is not derived\n  from a spec. It is read from the company's own distributed WordPress plugin — which is\n  a first-party client of the STN Video Publisher API — and confirmed against live\n  unauthenticated calls to the API host. Two distinct surfaces exist with two distinct\n  auth postures.\nsummary:\n  types: [none, custom-credential-pair]\n  api_key_in: [body]\n  oauth2_flows: []\n  bearer: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: none\n  type: none\n  api:\
  \ STN Video oEmbed API\n  base_url: https://embed.sendtonews.com/services/oembed\n  description: >-\n    The oEmbed 1.0 endpoint is public and unauthenticated. A GET with a `url` parameter\n    naming an embed.sendtonews.com resource returns a 200 oEmbed video payload with no\n    credential of any kind.\n  evidence:\n  - request: >-\n      GET https://embed.sendtonews.com/services/oembed?url=https%3A%2F%2Fembed.sendtonews.com%2Foembed%2F%3FSC%3D<share-code>&format=json\n    status: 200\n    content_type: application/json; charset=UTF-8\n    observed: '2026-08-12'\n- name: cid + authcode\n  type: custom-credential-pair\n  api: STN Video Publisher API\n  base_url: https://api.sendtonews.com/api/v1/\n  in: body\n  parameters:\n  - name: cid\n    description: Company ID issued by STN Video to a publisher account.\n  - name: authcode\n    description: Authentication Code issued alongside the Company ID.\n  transport: POST, application/x-www-form-urlencoded request body\n  verification_operation:\
  \ POST /api/v1/auth/verifycode\n  issuance: >-\n    Credentials are not self-serve. The publisher documentation directs integrators to\n    publishers@stnvideo.com to obtain a Company ID and Authentication Code, so the API is\n    customer-gated rather than open.\n  description: >-\n    Every STN Video Publisher API operation carries the same credential pair in the POST\n    body — there is no header scheme, no bearer token, no OAuth, and no scope model. The\n    plugin additionally sends non-credential telemetry fields (appName, appVersion,\n    cmsVersion, appComponent) on the verification call.\n  evidence:\n  - request: POST https://api.sendtonews.com/api/v1/auth/verifycode (no body)\n    status: 422\n    response: '{\"success\":false,\"code\":422,\"errors\":{\"authcode\":\"authcode is required\",\"cid\":\"cid is required\"}}'\n    observed: '2026-08-12'\n  - request: POST https://api.sendtonews.com/api/v1/players (no body)\n    status: 422\n    response: '{\"success\":false,\"code\"\
  :422,\"errors\":{\"authcode\":\"authcode is required\",\"cid\":\"cid is required\"}}'\n    observed: '2026-08-12'\n  - source: sendtonews/app/Controllers/AdminController.php (plugin v1.2.2)\n    kind: first-party client source\ngaps:\n- No published authentication reference page; the credential model had to be read out of\n  the provider's own plugin source.\n- Credentials are transmitted as body parameters on every call rather than exchanged for a\n  short-lived token.\n- No OAuth 2.0, no OpenID Connect, no scopes, no key rotation or revocation surface is\n  documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minute-media/refs/heads/main/authentication/minute-media-authentication.yml
summary_line: none/custom-credential-pair · 2 schemes
tags:
- Company
- Media
- Sports
- Advertising
- Video
- Publishing
- AdTech
- Content
- oEmbed
- Online Video Platform
---
