---
api_key_in:
- header
auth_types:
- apiKey
description: Crunchtime Inventory & Labor APIs authenticate with a per-environment API authentication token issued from Enterprise Manager, sent together with the customer site name, application user id and password. Tokens are scoped per environment (separate Test and Production tokens); a single token can access multiple API services within its environment, and grants access to data for all locations associated with that application user's Crunchtime site. There is no OAuth 2.0 / OpenID Connect flow and no scope surface — this is a token + named-application-user model, so no scopes/ artifact is emitted.
kind: authentication
layout: security
method: searched
name: Crunchtime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crunchtime secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crunchtime
provider_slug: crunchtime
scheme_count: 4
schemes:
- description: Per-environment (Test or Production) API token generated and managed in Enterprise Manager under Security > Application Users > API Tokens. Token value is shown only once at creation; can be regenerated or revoked. Tokens do not carry OAuth scopes.
  in: header
  name: authenticationtoken
  parameter: authenticationtoken
  sources:
  - https://developer.crunchtime.com/docs/getting-started-with-apis
  type: apiKey
- description: The Crunchtime site identifier — the portion of the customer URL before ".net-chef.com" (e.g. "eattacos" for eattacos.net-chef.com, "eattacos-test" for the test environment). Combined with the token to select the environment.
  in: field
  name: sitename
  parameter: sitename
  sources:
  - https://developer.crunchtime.com/docs/getting-started-with-apis
  type: apiKey
- description: Application User ID of a dedicated Crunchtime application user (e.g. "API User").
  in: field
  name: userid
  parameter: userid
  sources:
  - https://developer.crunchtime.com/docs/getting-started-with-apis
  type: apiKey
- description: Password for the Crunchtime application user.
  in: field
  name: password
  parameter: password
  sources:
  - https://developer.crunchtime.com/docs/getting-started-with-apis
  type: apiKey
slug: crunchtime-authentication
source_filename: crunchtime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.crunchtime.com/docs/getting-started-with-apis\ndocs: https://developer.crunchtime.com/docs/getting-started-with-apis\ndescription: >-\n  Crunchtime Inventory & Labor APIs authenticate with a per-environment API\n  authentication token issued from Enterprise Manager, sent together with the\n  customer site name, application user id and password. Tokens are scoped per\n  environment (separate Test and Production tokens); a single token can access\n  multiple API services within its environment, and grants access to data for\n  all locations associated with that application user's Crunchtime site. There is\n  no OAuth 2.0 / OpenID Connect flow and no scope surface — this is a token +\n  named-application-user model, so no scopes/ artifact is emitted.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: authenticationtoken\n  type: apiKey\n  in: header\n  parameter:\
  \ authenticationtoken\n  description: >-\n    Per-environment (Test or Production) API token generated and managed in\n    Enterprise Manager under Security > Application Users > API Tokens. Token\n    value is shown only once at creation; can be regenerated or revoked. Tokens\n    do not carry OAuth scopes.\n  sources:\n  - https://developer.crunchtime.com/docs/getting-started-with-apis\n- name: sitename\n  type: apiKey\n  in: field\n  parameter: sitename\n  description: >-\n    The Crunchtime site identifier — the portion of the customer URL before\n    \".net-chef.com\" (e.g. \"eattacos\" for eattacos.net-chef.com, \"eattacos-test\"\n    for the test environment). Combined with the token to select the environment.\n  sources:\n  - https://developer.crunchtime.com/docs/getting-started-with-apis\n- name: userid\n  type: apiKey\n  in: field\n  parameter: userid\n  description: Application User ID of a dedicated Crunchtime application user (e.g. \"API User\").\n  sources:\n  - https://developer.crunchtime.com/docs/getting-started-with-apis\n\
  - name: password\n  type: apiKey\n  in: field\n  parameter: password\n  description: Password for the Crunchtime application user.\n  sources:\n  - https://developer.crunchtime.com/docs/getting-started-with-apis\nnotes:\n  environments:\n    test: https://webservices-test.net-chef.com\n    production: https://webservices.net-chef.com\n  token_management: Enterprise Manager > Security > Application Users > API Tokens (add/edit/regenerate/revoke)\n  support: apiquestions@crunchtime.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchtime/refs/heads/main/authentication/crunchtime-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Restaurant Operations
- Inventory Management
- Labor & Scheduling
- Food Cost
- Kitchen Display
- Point of Sale
- Supply Chain
- Hospitality
- REST API
---
