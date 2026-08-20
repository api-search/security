---
api_key_in: []
api_specs:
- filename: lengow-channel-execution-openapi.yml
  format: yaml
  label: Lengow Channel Execution API
  slug: lengow-channel-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/openapi/lengow-channel-execution-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lengow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lengow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lengow
provider_slug: lengow
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lengow-channel-execution-openapi.yml
  type: http
slug: lengow-authentication
source_filename: lengow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/lengow-channel-execution-openapi.yml\ndocs: https://docs.lengow.io/#authentication\ndocs_secondary: https://api.lengow.io/docs/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  model: two-key credential exchange for a short-lived bearer session token\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lengow-channel-execution-openapi.yml\nflow:\n  step_1:\n    description: >-\n      Exchange the account's two long-lived API keys for a session token. Both keys are issued in the API\n      section of the Lengow account and are unique per (sub)account; generating a new pair automatically\n      revokes the previous one.\n    operation: POST https://api.lengow.io/access/get_token\n    body_params:\n    - name: access_token\n      required: true\n      description: Access token of the application, from the API section of the Lengow account\n    - name: secret\n   \
  \   required: true\n      description: Secret of the application, from the API section of the Lengow account\n    response: '{\"token\": \"<session token>\", \"account_id\": <int>}'\n  step_2:\n    description: >-\n      Send the session token on every subsequent request in an Authorization header. The docs show the\n      raw token value with no \"Bearer \" prefix in the curl examples, while the OpenAPI declares an\n      http/bearer scheme — clients should follow the docs example.\n    header: 'Authorization: ${TOKEN}'\n  step_3:\n    description: Check remaining session validity.\n    operation: GET https://api.lengow.io/me\n    returns: current session description including the expiration date of the session token\ntoken:\n  lifetime: 1 hour\n  refresh: re-call POST /access/get_token; the docs state it is unnecessary to request a token per request\n  rotation: generating new keys in the account UI revokes previously generated keys\n  subaccounts: API keys are per (sub)account, so each\
  \ subaccount authenticates separately\nfailure_modes:\n- status: 400\n  operation: POST /access/get_token\n  meaning: authentication error (bad access_token/secret pair)\n- status: 401\n  meaning: 'missing, invalid, or expired authentication token (example body: {\"error\": {\"message\": \"Missing authentication token\", \"code\": 401}})'\n- status: 403\n  meaning: 'invalid or expired session, or no token in headers (example body: {\"error\": {\"message\": \"No token in headers to access /orders API\", \"code\": 403}})'\nnot_supported:\n- oauth2\n- openIdConnect\n- mutualTLS\n- api key in query string\n- scopes / granular permissions (there is no scope surface; a session token carries the account's full API rights)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/authentication/lengow-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Software-as-a-Service
- E-Commerce
- Marketplaces
- Product Feeds
- Retail
- Advertising
- Order Management
- Price Intelligence
- France
---
