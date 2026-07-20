---
api_key_in:
- header
api_specs:
- filename: coinflow-openapi-original.json
  format: json
  label: Coinflow API
  slug: coinflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Coinflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coinflow secures its APIs with apiKey across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coinflow
provider_slug: coinflow
scheme_count: 7
schemes:
- description: The web3 wallet of the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key
  in: header
  name: wallet
  parameter: x-coinflow-auth-wallet
  sources:
  - openapi/coinflow-openapi-original.json
  type: apiKey
- description: The blockchain associated with the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key
  in: header
  name: blockchain
  parameter: x-coinflow-auth-blockchain
  sources:
  - openapi/coinflow-openapi-original.json
  type: apiKey
- description: The external identifier of the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key
  in: header
  name: userId
  parameter: x-coinflow-auth-user-id
  sources:
  - openapi/coinflow-openapi-original.json
  type: apiKey
- description: The API key of the merchant - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key
  in: header
  name: merchant
  parameter: Authorization
  sources:
  - openapi/coinflow-openapi-original.json
  type: apiKey
- description: The message signed by the users wallet
  in: header
  name: signedMessage
  parameter: x-coinflow-auth-signed-message
  sources:
  - openapi/coinflow-openapi-original.json
  type: apiKey
- description: The merchant ID the session should be generated for
  in: header
  name: merchantId
  parameter: x-coinflow-auth-merchant-id
  sources:
  - openapi/coinflow-openapi-original.json
  type: apiKey
- description: The session key generated for the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key
  in: header
  name: sessionKey
  parameter: x-coinflow-auth-session-key
  sources:
  - openapi/coinflow-openapi-original.json
  type: apiKey
slug: coinflow-authentication
source_filename: coinflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/coinflow-openapi-original.json\ndocs: https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    Multi-layered header auth. Server-to-server requests carry the merchant API\n    key in the Authorization header. End-user context is established either by a\n    session key (call get-session-key with x-coinflow-auth-user-id, then pass\n    x-coinflow-auth-session-key; session keys last 24 hours) or by web3 wallet\n    verification (x-coinflow-auth-wallet + x-coinflow-auth-blockchain, proven with\n    a signature in x-coinflow-auth-signed-message and confirmed via verify-token).\n    No OAuth2/OIDC.\n  session_ttl: 24 hours\nschemes:\n- name: wallet\n  type: apiKey\n  in: header\n  parameter: x-coinflow-auth-wallet\n  description: The web3 wallet of the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key\n\
  \  sources:\n  - openapi/coinflow-openapi-original.json\n- name: blockchain\n  type: apiKey\n  in: header\n  parameter: x-coinflow-auth-blockchain\n  description: The blockchain associated with the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key\n  sources:\n  - openapi/coinflow-openapi-original.json\n- name: userId\n  type: apiKey\n  in: header\n  parameter: x-coinflow-auth-user-id\n  description: The external identifier of the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key\n  sources:\n  - openapi/coinflow-openapi-original.json\n- name: merchant\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The API key of the merchant - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key\n  sources:\n  - openapi/coinflow-openapi-original.json\n- name: signedMessage\n  type: apiKey\n  in: header\n  parameter: x-coinflow-auth-signed-message\n\
  \  description: The message signed by the users wallet\n  sources:\n  - openapi/coinflow-openapi-original.json\n- name: merchantId\n  type: apiKey\n  in: header\n  parameter: x-coinflow-auth-merchant-id\n  description: The merchant ID the session should be generated for\n  sources:\n  - openapi/coinflow-openapi-original.json\n- name: sessionKey\n  type: apiKey\n  in: header\n  parameter: x-coinflow-auth-session-key\n  description: The session key generated for the end user - see https://docs.coinflow.cash/api-reference/api-reference/authentication/get-session-key\n  sources:\n  - openapi/coinflow-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/authentication/coinflow-authentication.yml
summary_line: apiKey · 7 schemes
tags:
- Company
- Crypto
- Payments
- Stablecoin
- USDC
- Checkout
- Payouts
- Marketplace
- Web3
- Fintech
---
