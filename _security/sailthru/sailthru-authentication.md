---
api_key_in:
- query
- formData
auth_types:
- apiKey
- requestSignature
description: ''
kind: authentication
layout: security
method: searched
name: Sailthru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sailthru secures its APIs with apiKey and requestSignature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sailthru
provider_slug: sailthru
scheme_count: 3
schemes:
- description: The unique identifier for the company account, sent on every request.
  in: query
  name: api_key
  parameter: api_key
  required: true
  type: apiKey
- algorithm: MD5
  description: MD5 hash of the account secret + api_key + format + the JSON-object parameter values, sorted alphabetically. Parameters must NOT be URL-encoded before the signature is generated, only after.
  in: query
  name: sig
  parameter: sig
  required: true
  type: requestSignature
- description: Response serialization; participates in the signature, so it is part of the authenticated request rather than a content-negotiation header.
  in: query
  name: format
  parameter: format
  required: true
  type: parameter
  values:
  - json
  - xml
slug: sailthru-authentication
source_filename: sailthru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://products.zetaglobal.com/sailthru/Content/developers/api-basics/technical.html\ndocs: https://products.zetaglobal.com/sailthru/Content/developers/api-basics/technical.html\napi: sailthru:sailthru-api\nnote: >-\n  Sailthru predates OpenAPI and publishes no machine-readable security scheme,\n  so this profile is read from the API technical-details page rather than\n  derived from a spec. Authentication is a shared-secret request-signing model:\n  every call carries the account's api_key plus a sig parameter that is an MD5\n  hash of the account secret concatenated with the alphabetically sorted values\n  of every request parameter. There is no OAuth 2.0, no OpenID Connect, no\n  bearer token and no scope surface — which is why scopes/ is deliberately\n  absent from this repo rather than empty.\nsummary:\n  types: [apiKey, requestSignature]\n  api_key_in: [query, formData]\n  oauth2_flows: []\n  scopes: false\n  mtls: false\n\
  schemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: The unique identifier for the company account, sent on every request.\n  required: true\n- name: sig\n  type: requestSignature\n  in: query\n  parameter: sig\n  algorithm: MD5\n  description: >-\n    MD5 hash of the account secret + api_key + format + the JSON-object\n    parameter values, sorted alphabetically. Parameters must NOT be\n    URL-encoded before the signature is generated, only after.\n  required: true\n- name: format\n  type: parameter\n  in: query\n  parameter: format\n  values: [json, xml]\n  description: >-\n    Response serialization; participates in the signature, so it is part of\n    the authenticated request rather than a content-negotiation header.\n  required: true\ntransport:\n  https_required: true\n  tls: TLS 1.2 or higher; SSL is not supported\n  encoding: UTF-8\ncredential_management:\n  console: API & Postbacks settings in the Sailthru application\n  ip_allowlist:\
  \ true\n  ip_allowlist_error: 'API error 4 — Disallowed IP'\n  rotation_policy: null\nfailure_modes:\n- {http_status: 401, api_error: 3, meaning: Invalid API key}\n- {http_status: 401, api_error: 5, meaning: Authentication failed}\n- {http_status: 403, api_error: 4, meaning: Disallowed IP}\n- {http_status: 400, api_error: 2, meaning: 'Missing HTTPS GET/POST parameter (e.g. api_key)'}\nwebhook_authentication:\n  mechanism: shared-secret signature\n  description: >-\n    API postbacks posted back to a customer-hosted URL carry api_key and a sig\n    that is a hash of the API key and all parameter values, so the receiver can\n    verify the call originated from Sailthru.\n  source: https://products.zetaglobal.com/sailthru/Content/developers/api-basics/postbacks.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sailthru/refs/heads/main/authentication/sailthru-authentication.yml
summary_line: apiKey/requestSignature · 3 schemes
tags:
- Company
- Email Marketing
- Marketing Automation
- Personalization
- Customer Data Platform
- Transactional Email
- SMS
- Push Notifications
- Retail
- Media and Publishing
---
