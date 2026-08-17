---
api_key_in:
- query
- body
api_specs:
- filename: neverbounce-account-api-openapi.yml
  format: yaml
  label: NeverBounce Account API
  slug: neverbounce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-account-api-openapi.yml
- filename: neverbounce-jobs-api-openapi.yml
  format: yaml
  label: NeverBounce Jobs API
  slug: neverbounce-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-jobs-api-openapi.yml
- filename: neverbounce-single-api-openapi.yml
  format: yaml
  label: NeverBounce Single API
  slug: neverbounce-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-single-api-openapi.yml
- filename: neverbounce-poe-api-openapi.yml
  format: yaml
  label: NeverBounce POE API
  slug: neverbounce-poe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-poe-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Neverbounce Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeverBounce secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NeverBounce
provider_slug: neverbounce
scheme_count: 1
schemes:
- description: 'Static per-integration API key. V4 keys are prefixed `secret_` followed by 32 characters. Created from the dashboard as a "Custom Integration App" (https://app.neverbounce.com/apps/custom-integration/new); the key can be reset from the same app overview page. The published OpenAPI definition declares this scheme as `sec0` (apiKey, in: query, name: key).'
  in: query
  name: sec0
  parameter: key
  sources:
  - openapi/neverbounce-account-api-openapi.yml
  - openapi/neverbounce-jobs-api-openapi.yml
  - openapi/neverbounce-poe-api-openapi.yml
  - openapi/neverbounce-single-api-openapi.yml
  - https://developers.neverbounce.com/reference/authentication
  type: apiKey
slug: neverbounce-authentication
source_filename: neverbounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.neverbounce.com/reference/authentication\ndocs: https://developers.neverbounce.com/reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - body\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: sec0\n  type: apiKey\n  in: query\n  parameter: key\n  description: >-\n    Static per-integration API key. V4 keys are prefixed `secret_` followed by 32\n    characters. Created from the dashboard as a \"Custom Integration App\"\n    (https://app.neverbounce.com/apps/custom-integration/new); the key can be reset from\n    the same app overview page. The published OpenAPI definition declares this scheme as\n    `sec0` (apiKey, in: query, name: key).\n  sources:\n  - openapi/neverbounce-account-api-openapi.yml\n  - openapi/neverbounce-jobs-api-openapi.yml\n  - openapi/neverbounce-poe-api-openapi.yml\n  - openapi/neverbounce-single-api-openapi.yml\n  - https://developers.neverbounce.com/reference/authentication\n\
  key_prefixes:\n- prefix: secret_\n  surface: v4 REST API\n  usage: >-\n    Server-side only. Grants access to account data and consumes verification credits.\n    Accepted in the query string (`?key=`), in an `application/x-www-form-urlencoded`\n    body, or in an `application/json` body.\n  note: >-\n    NeverBounce explicitly warns that the standard API is not usable from a browser — CORS\n    is not enabled — because the key would be exposed client-side.\n- prefix: public_\n  surface: JavaScript widget\n  usage: >-\n    Browser-safe publishable key for the NeverBounce JS widget only. Keys starting with\n    `public_` cannot authenticate the standard API, and `secret_` keys cannot drive the\n    widget.\n  source: https://developers.neverbounce.com/reference/widget-overview\n- prefix: webhook_secret_\n  surface: single/check webhook URLs\n  usage: >-\n    Key embedded in a generated webhook URL (created at\n    https://app.neverbounce.com/apps/webhook/new) so third-party tools can call\n\
  \    `/single/check` without code. NeverBounce documents these URLs as sensitive — they\n    carry a live key and must not be used client-side.\n  source: https://developers.neverbounce.com/reference/single-webhooks\ntransport:\n  https_only: true\n  interchangeable_verbs: true\n  accepted_content_types:\n  - application/x-www-form-urlencoded\n  - application/json\n  note: >-\n    v4 accepts GET and POST interchangeably; PUT, DELETE, HEAD and OPTIONS are not\n    supported. See https://developers.neverbounce.com/reference/encoding-requests\nfailure_modes:\n- status: auth_failure\n  http_status: 200\n  meaning: >-\n    Request could not be authenticated. Most often a legacy V3 username/secret being sent\n    to a V4 endpoint — V3 credentials do not work on V4.\n- status: bad_referrer\n  http_status: 200\n  meaning: >-\n    Request originated from a domain or IP not listed in the app's Trusted Domains\n    (widget and webhook apps).\nnotes:\n- >-\n  There is no OAuth 2.0 or OpenID Connect\
  \ surface. Authentication is a single static API\n  key per integration app, rotated by resetting the key in the dashboard.\n- >-\n  Authentication failures are returned inside a HTTP 200 body via the `status` property,\n  not as a 401 — see errors/neverbounce-problem-types.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/authentication/neverbounce-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Verification
- Email Validation
- Email Hygiene
- Deliverability
- Marketing
- List Cleaning
- Data Quality
- ZoomInfo
---
