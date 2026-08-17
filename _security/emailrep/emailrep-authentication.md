---
api_key_in:
- header
api_specs:
- filename: emailrep-reports-api-openapi.yml
  format: yaml
  label: EmailRep Reports API
  slug: emailrep-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailrep/refs/heads/main/openapi/emailrep-reports-api-openapi.yml
- filename: emailrep-reputation-api-openapi.yml
  format: yaml
  label: EmailRep Reputation API
  slug: emailrep-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailrep/refs/heads/main/openapi/emailrep-reputation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Emailrep Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmailRep secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EmailRep
provider_slug: emailrep
scheme_count: 1
schemes:
- description: 'EmailRep API key. The docs show it verbatim as `Key: [your api key]` alongside the request line `GET https://emailrep.io/{email}`. The provider''s own OpenAPI names this scheme simply `Key` and applies it to POST /report; the refined specs in this repo name it `ApiKeyAuth`. Same header, same value.'
  in: header
  invalid_key_status: 401
  name: ApiKeyAuth
  parameter: Key
  signup: https://emailrep.io/free
  sources:
  - openapi/emailrep-reports-api-openapi.yml
  - openapi/emailrep-reputation-api-openapi.yml
  - openapi/_original/emailrep-alpha-api-openapi.json
  - https://docs.sublime.security/reference/emailrep-introduction
  type: apiKey
slug: emailrep-authentication
source_filename: emailrep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://docs.sublime.security/reference/emailrep-introduction\nsource: >-\n  https://docs.sublime.security/reference/emailrep-introduction, upgraded from the derived\n  baseline over openapi/emailrep-reports-api-openapi.yml and\n  openapi/emailrep-reputation-api-openapi.yml, and cross-checked against the provider's own\n  OpenAPI at openapi/_original/emailrep-alpha-api-openapi.json.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: none\n  mtls: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Key\n  description: >-\n    EmailRep API key. The docs show it verbatim as `Key: [your api key]` alongside the request\n    line `GET https://emailrep.io/{email}`. The provider's own OpenAPI names this scheme simply\n    `Key` and applies it to POST /report; the refined specs in this repo name it `ApiKeyAuth`.\n    Same header, same value.\n  signup: https://emailrep.io/free\n\
  \  invalid_key_status: 401\n  sources:\n  - openapi/emailrep-reports-api-openapi.yml\n  - openapi/emailrep-reputation-api-openapi.yml\n  - openapi/_original/emailrep-alpha-api-openapi.json\n  - https://docs.sublime.security/reference/emailrep-introduction\nsecond_factor:\n  name: User-Agent\n  required: true\n  type: http-header\n  missing_status: 403\n  description: >-\n    NOT an auth scheme in any spec, but functionally a gate: \"Each request to the API must be\n    accompanied by a user agent request header ... A missing user agent will result in an HTTP 403\n    response. The user agent should accurately describe the nature of the API consumer such that\n    it can be clearly identified in the request. Not doing so may result in the request being\n    blocked.\" An agent that omits it never reaches the key check.\n  source: https://docs.sublime.security/reference/emailrep-introduction\nanonymous_access:\n  documented: true\n  actual: false\n  detail: >-\n    The docs state a key is\
  \ optional. Production disagrees. An anonymous\n    GET https://emailrep.io/bill@microsoft.com on 2026-08-13 returned HTTP 429 with\n    {\"status\": \"fail\", \"reason\": \"the unauthenticated API is currently disabled. please use an\n    API key\"}. Both operations should be treated as key-required.\n  x-evidence:\n    fetched: '2026-08-13'\n    url: https://emailrep.io/bill@microsoft.com\n    http_status: 429\nper_operation:\n  - operation: queryEmailReputation\n    security: 'ApiKeyAuth (documented optional; enforced in production)'\n  - operation: reportEmail\n    security: \"ApiKeyAuth (required — the provider's own spec applies `security: [{Key: []}]` to this operation only)\"\nexample_request: |\n  GET https://emailrep.io/{email}\n  Key: [your api key]\n  User-Agent: [your app name]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailrep/refs/heads/main/authentication/emailrep-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Email
- Email Reputation
- Threat Intelligence
- Phishing
- Fraud Prevention
- Anti-Abuse
- Deliverability
- Risk Scoring
- Public APIs
---
