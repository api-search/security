---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: commutescout-com-tools-api-openapi.yml
  format: yaml
  label: CommuteScout Tools API
  slug: commutescout-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commutescout-com/openapi/commutescout-com-tools-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CommuteScout Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommuteScout secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CommuteScout
provider_slug: commutescout-com
scheme_count: 2
schemes:
- description: 'A key from Settings on commutescout.com/map. Optional: without one, per-address limits apply.'
  in: header
  key_prefix: cs_live_
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/commutescout-com-openapi.yml
  - https://commutescout.com/developers
  type: apiKey
- description: 'The same key as a bearer token (Authorization: Bearer cs_live_...).'
  name: BearerKey
  scheme: bearer
  sources:
  - openapi/commutescout-com-openapi.yml
  - https://commutescout.com/developers
  type: http
slug: commutescout-com-authentication
source_filename: commutescout-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commutescout.com/developers\ndocs: https://commutescout.com/developers\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  optional: true\n  note: Keys are optional. Without a key, requests are limited per network address; a key moves the caller onto its own limits.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  key_prefix: cs_live_\n  description: 'A key from Settings on commutescout.com/map. Optional: without one, per-address limits apply.'\n  sources:\n  - openapi/commutescout-com-openapi.yml\n  - https://commutescout.com/developers\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: 'The same key as a bearer token (Authorization: Bearer cs_live_...).'\n  sources:\n  - openapi/commutescout-com-openapi.yml\n  - https://commutescout.com/developers\nkey_management:\n  issuance: 'Every key belongs to a signed-in account: open the live map, choose\
  \ Settings in the rail, sign in with Google or an email link, and create a key under API keys. The key is shown once.'\n  limits: An account holds up to five active keys and creates up to ten a day.\n  revocation: Revoking a key stops it within a minute.\n  invalid_key_behavior: 401 invalid_key; there is no silent fallback to keyless.\n  guidance: Do not put a key in a web page or a mobile app. Call keyless from browsers (the API allows cross-origin reads) or keep the key on a server you control.\n"
source_yaml_url: https://artifacts.apis.io/commutescout-com/authentication/commutescout-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Traffic
- Road Conditions
- Transportation
- Navigation
- Route Planning
- Maps
- MCP
- Open Source
---
