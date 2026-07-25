---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Jpx Authentication
name_suffix: Authentication
oauth_flows: []
overview: JPX (Japan Exchange Group) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JPX (Japan Exchange Group)
provider_slug: jpx
scheme_count: 1
schemes:
- description: All J-Quants API V2 requests authenticate with an API key sent in the x-api-key header. Keys are issued from the dashboard (Settings > API Key, https://jpx-jquants.com/dashboard/api-keys) after registering and subscribing to a plan (Free/Light/Standard/Premium). The key itself has no expiration date; re-issuance and deletion are possible from the dashboard.
  in: header
  name: apiKey
  parameter: x-api-key
  type: apiKey
slug: jpx-authentication
source_filename: jpx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://jpx-jquants.com/en/spec/quickstart\ndocs: https://jpx-jquants.com/en/spec/quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >-\n      All J-Quants API V2 requests authenticate with an API key sent in the\n      x-api-key header. Keys are issued from the dashboard (Settings > API Key,\n      https://jpx-jquants.com/dashboard/api-keys) after registering and\n      subscribing to a plan (Free/Light/Standard/Premium). The key itself has\n      no expiration date; re-issuance and deletion are possible from the\n      dashboard.\nnotes: >-\n  V1's token method (ID token / refresh token via /v1/token/auth_user and\n  /v1/token/auth_refresh) is abolished in V2. The official jquants CLI offers a\n  browser login (jquants login) that authenticates against the J-Quants account\n  via Cognito\
  \ OAuth2 PKCE and stores the API key in\n  ~/.config/jquants/credentials.json; the API itself is key-authenticated, and\n  there is no OAuth scope surface on api.jquants.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jpx/refs/heads/main/authentication/jpx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial
- Market Data
- Stocks
- Exchange
- Trading
- Derivatives
- Indices
- Reference Data
- Japan
---
