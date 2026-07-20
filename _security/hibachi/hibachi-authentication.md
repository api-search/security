---
api_key_in:
- header
api_specs:
- filename: hibachi-openapi.yml
  format: yaml
  label: Hibachi API
  slug: hibachi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibachi/refs/heads/main/openapi/hibachi-openapi.yml
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Hibachi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hibachi secures its APIs with apiKey and signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hibachi
provider_slug: hibachi
scheme_count: 1
schemes:
- description: API key identifying the account, passed in the Authorization header. Required for all endpoints except the public /market and /exchange endpoints. The API key does NOT sign requests.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/hibachi-openapi.yml
  type: apiKey
slug: hibachi-authentication
source_filename: hibachi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hibachi-openapi.yml\ndocs: https://api-doc.hibachi.xyz/\nsummary:\n  types:\n  - apiKey\n  - signature\n  api_key_in:\n  - header\n  signing:\n  - ecdsa\n  - hmac\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    API key identifying the account, passed in the Authorization header. Required for all\n    endpoints except the public /market and /exchange endpoints. The API key does NOT sign\n    requests.\n  sources:\n  - openapi/hibachi-openapi.yml\nsigning:\n  description: >-\n    Order, withdraw, and transfer payloads must additionally carry a `signature` field (65 bytes)\n    generated from the account's private/secret key. Trustless accounts (created by connecting a\n    crypto wallet) sign with an ECDSA private key; exchange-managed accounts (created via email or\n    social login) sign with an HMAC secret key. The signature is computed over a defined\
  \ byte\n    layout per operation (e.g. withdraw: assetId + quantity + maxFees).\n  methods:\n  - id: ecdsa\n    account_type: trustless\n    note: ECDSA signature over the operation payload; NOT the crypto wallet's private key.\n  - id: hmac\n    account_type: exchange-managed\n    note: HMAC signature using the account's secret key.\n  signed_operations:\n  - openapi/hibachi-openapi.yml#submitWithdraw\n  - openapi/hibachi-openapi.yml#submitTransfer\n  - openapi/hibachi-openapi.yml#placeOrder\n  - openapi/hibachi-openapi.yml#placeOrdersBatch\n  - openapi/hibachi-openapi.yml#modifyOrder\n  - openapi/hibachi-openapi.yml#cancelOrder\n  - openapi/hibachi-openapi.yml#cancelAllOrders\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hibachi/refs/heads/main/authentication/hibachi-authentication.yml
summary_line: apiKey/signature · 1 scheme
tags:
- Company
- Defi
- Cryptocurrency
- Exchange
- Perpetual Futures
- Trading
- Derivatives
- Stablecoin
- WebSocket
- Blockchain
---
