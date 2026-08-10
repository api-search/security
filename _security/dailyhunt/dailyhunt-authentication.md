---
api_key_in:
- header
- body
api_specs:
- filename: dailyhunt-catalog-api-openapi.yml
  format: yaml
  label: Dailyhunt Catalog API
  slug: dailyhunt-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-catalog-api-openapi.yml
- filename: dailyhunt-channels-api-openapi.yml
  format: yaml
  label: Dailyhunt Channels API
  slug: dailyhunt-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-channels-api-openapi.yml
- filename: dailyhunt-content-fetch-api-openapi.yml
  format: yaml
  label: Dailyhunt Content Fetch API
  slug: dailyhunt-content-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-content-fetch-api-openapi.yml
- filename: dailyhunt-cricket-api-openapi.yml
  format: yaml
  label: Dailyhunt Cricket API
  slug: dailyhunt-cricket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-cricket-api-openapi.yml
- filename: dailyhunt-feedback-api-openapi.yml
  format: yaml
  label: Dailyhunt Feedback API
  slug: dailyhunt-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-feedback-api-openapi.yml
- filename: dailyhunt-languages-api-openapi.yml
  format: yaml
  label: Dailyhunt Languages API
  slug: dailyhunt-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-languages-api-openapi.yml
- filename: dailyhunt-products-api-openapi.yml
  format: yaml
  label: Dailyhunt Products API
  slug: dailyhunt-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-products-api-openapi.yml
- filename: dailyhunt-tracking-api-openapi.yml
  format: yaml
  label: Dailyhunt Tracking API
  slug: dailyhunt-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/openapi/dailyhunt-tracking-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dailyhunt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dailyhunt secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dailyhunt
provider_slug: dailyhunt
scheme_count: 3
schemes:
- description: The partner API key issued by Dailyhunt at onboarding, sent on every Content Syndication call in the Authorization header with the literal prefix `key=`.
  docs: https://api-syndication.dailyhunt.in/
  format: key=<API Key>
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/dailyhunt-content-syndication-openapi.yml
  type: apiKey
- algorithm: HMAC-SHA1
  description: Every Content Syndication request additionally carries a request signature. The signature base string is built by appending a `ts` timestamp query parameter, URL-encoding every parameter key and value, sorting the parameters lexicographically on the encoded key, joining them as `key=value` pairs, and appending the uppercased HTTP method. That string is signed with the partner Secret Key using HMAC-SHA1 and Base64-encoded into the `Signature` header. Dailyhunt publishes worked JavaScript and Java reference implementations in the Partner Integration Reference.
  docs: https://api-syndication.dailyhunt.in/
  encoding: base64
  in: header
  name: RequestSignature
  parameter: Signature
  sources:
  - openapi/dailyhunt-content-syndication-openapi.yml
  type: apiKey
- description: The E-Commerce Shopping Catalog API authenticates with a vendor access_token passed as a field in the JSON request body of every catalog and batch call. The vendor must already be registered in the Dailyhunt system.
  docs: https://developer.dailyhunt.in/ads/docs/shopping-catalog/
  in: body
  name: VendorAccessToken
  parameter: access_token
  sources:
  - openapi/dailyhunt-shopping-catalog-openapi.yml
  type: apiKey
slug: dailyhunt-authentication
source_filename: dailyhunt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/dailyhunt-content-syndication-openapi.yml, openapi/dailyhunt-shopping-catalog-openapi.yml\ndocs: https://api-syndication.dailyhunt.in/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - body\n  oauth2_flows: []\n  self_service: false\n  provisioning: >-\n    Credentials are not self-service. Dailyhunt provisions an API Key, a Secret Key and a Partner\n    Code during partner onboarding and shares them over email. The E-Commerce Shopping Catalog API\n    requires the vendor to be registered first and issues a vendor access_token.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'key=<API Key>'\n  description: >-\n    The partner API key issued by Dailyhunt at onboarding, sent on every Content Syndication call in\n    the Authorization header with the literal prefix `key=`.\n  sources:\n  - openapi/dailyhunt-content-syndication-openapi.yml\n  docs: https://api-syndication.dailyhunt.in/\n\
  - name: RequestSignature\n  type: apiKey\n  in: header\n  parameter: Signature\n  algorithm: HMAC-SHA1\n  encoding: base64\n  description: >-\n    Every Content Syndication request additionally carries a request signature. The signature base\n    string is built by appending a `ts` timestamp query parameter, URL-encoding every parameter key\n    and value, sorting the parameters lexicographically on the encoded key, joining them as\n    `key=value` pairs, and appending the uppercased HTTP method. That string is signed with the\n    partner Secret Key using HMAC-SHA1 and Base64-encoded into the `Signature` header. Dailyhunt\n    publishes worked JavaScript and Java reference implementations in the Partner Integration\n    Reference.\n  sources:\n  - openapi/dailyhunt-content-syndication-openapi.yml\n  docs: https://api-syndication.dailyhunt.in/\n- name: VendorAccessToken\n  type: apiKey\n  in: body\n  parameter: access_token\n  description: >-\n    The E-Commerce Shopping Catalog API authenticates\
  \ with a vendor access_token passed as a field in\n    the JSON request body of every catalog and batch call. The vendor must already be registered in\n    the Dailyhunt system.\n  sources:\n  - openapi/dailyhunt-shopping-catalog-openapi.yml\n  docs: https://developer.dailyhunt.in/ads/docs/shopping-catalog/\nidentity:\n  partner_user_id:\n    parameter: puid\n    required: true\n    description: >-\n      A partner-supplied unique identifier for the end user consuming Dailyhunt content (for example\n      a device identifier). Required on every Content Syndication call. Dailyhunt maps it to an\n      internal user id to build a personalization profile.\n  session_cookie:\n    name: dhFeedV1\n    description: >-\n      Dailyhunt returns a per-user dhFeedV1 cookie on the first API response. The partner must\n      persist it per user and replay it on subsequent calls; Dailyhunt regenerates it if missing or\n      expired and rejects requests carrying an invalid one. It avoids repeated puid-to-internal-id\n\
  \      lookups.\n    ttl: one month initially (Dailyhunt notes this may change)\nnotes:\n- No OAuth 2.0 or OpenID Connect surface is published; there is no scope model, so no scopes/\n  artifact is emitted for this provider.\n- No self-service developer signup exists for the Content Syndication API. The only self-service\n  signup on the estate is the Dailyhunt Direct advertising console at https://direct.dailyhunt.in/login.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - {url: 'https://api-syndication.dailyhunt.in/', http_status: 200}\n  - {url: 'https://developer.dailyhunt.in/ads/docs/shopping-catalog/', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailyhunt/refs/heads/main/authentication/dailyhunt-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- News
- Media
- Content Syndication
- Content
- Advertising
- Video
- Localization
- India
- Mobile
---
