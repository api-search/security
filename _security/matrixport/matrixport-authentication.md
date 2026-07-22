---
api_key_in:
- header
- query
api_specs:
- filename: matrixport-bitcom-openapi.yml
  format: yaml
  label: bit.com v1 API
  slug: bitcom-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-bitcom-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Matrixport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Matrixport secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Matrixport
provider_slug: matrixport
scheme_count: 3
schemes:
- description: Account access key identifying the caller.
  in: header
  name: ApiKeyAuth
  parameter: X-Bit-Access-Key
  sources:
  - openapi/matrixport-bitcom-openapi.yml
  type: apiKey
- description: Millisecond request timestamp included in the signed payload (guards against replay).
  in: query
  name: ApiTimestamp
  parameter: timestamp
  sources:
  - openapi/matrixport-bitcom-openapi.yml
  type: apiKey
- description: HMAC-SHA256 signature over the sorted request parameters, keyed with the account secret key.
  in: query
  name: ApiSignature
  parameter: signature
  sources:
  - openapi/matrixport-bitcom-openapi.yml
  type: apiKey
slug: matrixport-authentication
source_filename: matrixport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.bit.com/docs/en-us/spot.html#authentication\nsdk_source: https://github.com/bitcom-exchange/bitcom-go-api\ndocs: https://www.bit.com/docs/en-us/spot.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  model: >-\n    Access-key + HMAC-SHA256 request signing. Each private request carries the account access key,\n    a millisecond timestamp, and a signature computed by HMAC-SHA256 over the sorted request\n    parameters using the account secret key. Public market-data endpoints require no auth. API keys\n    (access key + secret key) are created in the bit.com account console.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Bit-Access-Key\n  description: Account access key identifying the caller.\n  sources: [openapi/matrixport-bitcom-openapi.yml]\n- name: ApiTimestamp\n  type: apiKey\n  in: query\n  parameter: timestamp\n  description: Millisecond request\
  \ timestamp included in the signed payload (guards against replay).\n  sources: [openapi/matrixport-bitcom-openapi.yml]\n- name: ApiSignature\n  type: apiKey\n  in: query\n  parameter: signature\n  description: HMAC-SHA256 signature over the sorted request parameters, keyed with the account secret key.\n  sources: [openapi/matrixport-bitcom-openapi.yml]\nwebsocket_auth:\n  endpoint: /v1/ws/auth\n  description: >-\n    Private WebSocket channels (order, user_trade, um_account) are authenticated with a token\n    obtained from GET /v1/ws/auth, then sent in the subscribe message on wss://ws.bit.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/authentication/matrixport-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Crypto Finance
- Cryptocurrency Exchange
- Trading
- Derivatives
- Options
- Futures
- Perpetuals
- WebSocket
- REST API
---
