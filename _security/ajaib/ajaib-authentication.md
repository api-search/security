---
api_key_in:
- header
api_specs:
- filename: ajaib-market-info-api-openapi.yml
  format: yaml
  label: Ajaib Market Info API
  slug: ajaib-market-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-market-info-api-openapi.yml
- filename: ajaib-spot-trading-api-openapi.yml
  format: yaml
  label: Ajaib Spot Trading API
  slug: ajaib-spot-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-spot-trading-api-openapi.yml
- filename: ajaib-wallet-api-openapi.yml
  format: yaml
  label: Ajaib Wallet API
  slug: ajaib-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-wallet-api-openapi.yml
auth_types:
- apiKey
- signed-request
description: ''
kind: authentication
layout: security
method: searched
name: Ajaib Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ajaib secures its APIs with apiKey and signed-request across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ajaib
provider_slug: ajaib
scheme_count: 3
schemes:
- description: The API key generated for the exchange client by Ajaib.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/ajaib-coin-exchange-openapi.yml
  type: apiKey
- algorithm: ECDSASHA256
  description: Signature over the concatenation of timestamp + method + requestPath + queryParam + requestBody, signed with the client's private key.
  in: header
  name: SignatureAuth
  parameter: X-SIGNATURE
  sources:
  - openapi/ajaib-coin-exchange-openapi.yml
  type: apiKey
- description: Unix timestamp in milliseconds, UTC timezone.
  in: header
  name: TimestampAuth
  parameter: X-TIMESTAMP
  sources:
  - openapi/ajaib-coin-exchange-openapi.yml
  type: apiKey
slug: ajaib-authentication
source_filename: ajaib-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://ajaib.gitbook.io/coin-exchange/getting-started/authentication\ndocs: https://ajaib.gitbook.io/coin-exchange/getting-started/authentication\nsummary:\n  types: [apiKey, signed-request]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Ajaib Coin Exchange uses an issued API key plus a per-request ECDSA-SHA256\n    request signature. There is no OAuth 2.0 or OpenID Connect surface, so no\n    scopes/ artifact is emitted.\nprovisioning:\n  self_service: false\n  process: >-\n    The client generates an ECDSASHA256 keypair, then emails the public key to\n    tech@ajaib.co.id. Ajaib returns an auto-generated API key bound to that\n    public key and to the client's identity as an exchange client.\n  contact: tech@ajaib.co.id\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-API-KEY\n    description: The API key generated for the exchange client by Ajaib.\n    sources: [openapi/ajaib-coin-exchange-openapi.yml]\n\
  \  - name: SignatureAuth\n    type: apiKey\n    in: header\n    parameter: X-SIGNATURE\n    algorithm: ECDSASHA256\n    description: >-\n      Signature over the concatenation of timestamp + method + requestPath +\n      queryParam + requestBody, signed with the client's private key.\n    sources: [openapi/ajaib-coin-exchange-openapi.yml]\n  - name: TimestampAuth\n    type: apiKey\n    in: header\n    parameter: X-TIMESTAMP\n    description: Unix timestamp in milliseconds, UTC timezone.\n    sources: [openapi/ajaib-coin-exchange-openapi.yml]\nsigning:\n  algorithm: ECDSASHA256\n  payload: timestamp + method + requestPath + queryParam + requestBody\n  rules:\n    - method must be uppercase (GET, POST, PUT, DELETE)\n    - requestPath must have a leading slash and no trailing slash, e.g. /api/v1/order\n    - queryParam is all query parameters joined with '&', no spaces or newlines\n    - requestBody is the JSON body with all newlines and spaces removed\n    - the timestamp signed must equal\
  \ the X-TIMESTAMP header value\n  failure: HTTP 403 with error \"invalid_client\"\npublic_operations:\n  - getServerTime\n  - getExchangeInfo\nauthenticated_operations:\n  - getDepth\n  - getPrice\n  - getPortfolio\n  - getTrades\n  - getOrder\n  - getOpenOrders\n  - createOrder\n  - createSelfTradingOrder\n  - createBatchOrders\n  - cancelOrder\n  - cancelBatchOrders\n  - cancelAllOpenOrders\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/authentication/ajaib-authentication.yml
summary_line: apiKey/signed-request · 3 schemes
tags:
- Company
- Financial-Services
- Investing
- Brokerage
- Trading
- Cryptocurrency
- Crypto Exchange
- Stocks
- Mutual Funds
- Fintech
- Indonesia
- Wealth Management
---
