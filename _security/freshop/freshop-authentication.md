---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Freshop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshop secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshop
provider_slug: freshop
scheme_count: 1
schemes:
- evidence:
  - 'GET /1/stores -> 400 {"error_code":"invalid_input","error_message":"app_key: is required"}'
  - 'GET /1/stores?app_key=bad_key_test -> 400 "app_key: bad_key_test is invalid"'
  in: query
  name: appKey
  parameter: app_key
  required: true
  sources:
  - live https://api.freshop.com
  type: apiKey
slug: freshop-authentication
source_filename: freshop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: live probe of https://api.freshop.com (missing/invalid app_key responses)\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  api_key_names: [app_key]\n  notes: >-\n    The Freshop API authenticates every request with an application key passed\n    as the `app_key` query-string parameter. A missing key returns HTTP 400\n    `{\"error_code\":\"invalid_input\",\"error_message\":\"app_key: is required\"}`;\n    an invalid key returns HTTP 400 `\"app_key: <value> is invalid\"`. User- and\n    session-scoped calls additionally accept a `token` parameter obtained from\n    the login/session endpoints (not verifiable without credentials).\nschemes:\n  - name: appKey\n    type: apiKey\n    in: query\n    parameter: app_key\n    required: true\n    sources: [live https://api.freshop.com]\n    evidence:\n      - 'GET /1/stores -> 400 {\"error_code\":\"invalid_input\",\"error_message\":\"app_key: is required\"}'\n      - 'GET /1/stores?app_key=bad_key_test\
  \ -> 400 \"app_key: bad_key_test is invalid\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshop/refs/heads/main/authentication/freshop-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Grocery
- eCommerce
- Retail
- Online Shopping
- Fulfillment
- Delivery
- NCR Voyix
---
