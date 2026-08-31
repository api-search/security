---
api_key_in:
- query
- header
api_specs:
- filename: tiingo-boats-api-openapi.yml
  format: yaml
  label: Tiingo BOATS API
  slug: tiingo-boats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-boats-api-openapi.yml
- filename: tiingo-corporate-actions-api-openapi.yml
  format: yaml
  label: Tiingo Corporate Actions API
  slug: tiingo-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-corporate-actions-api-openapi.yml
- filename: tiingo-crypto-api-openapi.yml
  format: yaml
  label: Tiingo Crypto API
  slug: tiingo-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-crypto-api-openapi.yml
- filename: tiingo-crypto-yield-api-openapi.yml
  format: yaml
  label: Tiingo Crypto Yield API
  slug: tiingo-crypto-yield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-crypto-yield-api-openapi.yml
- filename: tiingo-end-of-day-api-openapi.yml
  format: yaml
  label: Tiingo End Of Day API
  slug: tiingo-end-of-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-end-of-day-api-openapi.yml
- filename: tiingo-equity-realtime-api-openapi.yml
  format: yaml
  label: Tiingo Equity Realtime API
  slug: tiingo-equity-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-equity-realtime-api-openapi.yml
- filename: tiingo-forex-api-openapi.yml
  format: yaml
  label: Tiingo Forex API
  slug: tiingo-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-forex-api-openapi.yml
- filename: tiingo-fund-fees-api-openapi.yml
  format: yaml
  label: Tiingo Fund Fees API
  slug: tiingo-fund-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-fund-fees-api-openapi.yml
- filename: tiingo-fundamentals-api-openapi.yml
  format: yaml
  label: Tiingo Fundamentals API
  slug: tiingo-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-fundamentals-api-openapi.yml
- filename: tiingo-iex-api-openapi.yml
  format: yaml
  label: Tiingo IEX API
  slug: tiingo-iex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-iex-api-openapi.yml
- filename: tiingo-news-api-openapi.yml
  format: yaml
  label: Tiingo News API
  slug: tiingo-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-news-api-openapi.yml
- filename: tiingo-small-exchange-api-openapi.yml
  format: yaml
  label: Tiingo Small Exchange API
  slug: tiingo-small-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-small-exchange-api-openapi.yml
- filename: tiingo-utilities-api-openapi.yml
  format: yaml
  label: Tiingo Utilities API
  slug: tiingo-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-utilities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tiingo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tiingo secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tiingo
provider_slug: tiingo
scheme_count: 3
schemes:
- in: query
  name: apiTokenQuery
  parameter: token
  sources:
  - openapi/tiingo-openapi.yml
  type: apiKey
- format: Token <api-token>
  in: header
  name: apiTokenHeader
  parameter: Authorization
  sources:
  - openapi/tiingo-openapi.yml
  type: apiKey
- in: message
  name: websocketAuthorization
  notes: JSON field on every WebSocket subscribe/unsubscribe request.
  parameter: authorization
  sources:
  - asyncapi/tiingo-websockets-asyncapi.yml
  type: apiKey
slug: tiingo-authentication
source_filename: tiingo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\ndocs: https://www.tiingo.com/documentation/general/connecting\nsource: https://www.tiingo.com/documentation/general/connecting\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - header\n  oauth2_flows: []\nnotes: Every account is assigned a single API token used in place of username/password. REST accepts the token either\n  directly in the URL (?token=...) or in the Authorization header formatted as 'Token <token>'. WebSocket subscribe/unsubscribe\n  requests carry the token in the 'authorization' field of the JSON payload. Token rotation is available on the\n  account Token page (announced in the 2026-05-12 changelog). No OAuth surface.\nschemes:\n- name: apiTokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/tiingo-openapi.yml\n- name: apiTokenHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Token <api-token>\n  sources:\n  - openapi/tiingo-openapi.yml\n- name:\
  \ websocketAuthorization\n  type: apiKey\n  in: message\n  parameter: authorization\n  notes: JSON field on every WebSocket subscribe/unsubscribe request.\n  sources:\n  - asyncapi/tiingo-websockets-asyncapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/authentication/tiingo-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Fintech
- Market Data
- Stocks
- Crypto
- FX
- News
- Fundamentals
- WebSockets
---
