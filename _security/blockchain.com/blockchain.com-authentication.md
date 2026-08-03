---
api_key_in:
- header
api_specs:
- filename: blockchain.com-exchange-openapi.yml
  format: yaml
  label: Blockchain.com Exchange REST API
  slug: blockchaincom-exchange-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-exchange-openapi.yml
- filename: blockchain.com-pay-partner-api-openapi.yml
  format: yaml
  label: Blockchain.com Pay Partner API
  slug: blockchaincom-pay-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-pay-partner-api-openapi.yml
- filename: blockchain.com-nft-market-api-swagger.json
  format: json
  label: Blockchain.com NFT Market API
  slug: blockchaincom-nft-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-nft-market-api-swagger.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Blockchain.Com Authentication
name_suffix: Authentication
oauth_flows:
- bearer token (authorization endpoints not publicly documented)
overview: Blockchain.com secures its APIs with apiKey and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the bearer token (authorization endpoints not publicly documented) flow(s).
provider_name: Blockchain.com
provider_slug: blockchain.com
scheme_count: 5
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Token
  sources:
  - openapi/blockchain.com-exchange-openapi.yml
  type: apiKey
- description: Partner's public API key. Required on all endpoints to identify the partner.
  in: header
  name: PublicApiKeyAuth
  parameter: X-Public-API-Key
  sources:
  - openapi/blockchain.com-pay-partner-api-openapi.yml
  type: apiKey
- description: Partner's private API key. Required on order endpoints; indicates a server-to-server call.
  in: header
  name: PrivateApiKeyAuth
  parameter: X-Private-API-Key
  sources:
  - openapi/blockchain.com-pay-partner-api-openapi.yml
  type: apiKey
- description: OAuth 2.0 resource gateway for reading a consenting user's Blockchain.com custodial wallet transactions and balances. Documented only in prose; no OpenAPI and no RFC 8414 / RFC 9728 discovery document is published.
  in: header
  name: OAuth2 Bearer
  parameter: Authorization
  resource_server: https://api.blockchain.info/partner-resource-gateway
  scopes:
  - read_transactions
  - read_balance
  scopes_artifact: scopes/blockchain.com-scopes.yml
  sources:
  - https://docs.blockchain.com/oauth-resources/oauth-resources.md
  token_type: bearer
  type: oauth2
- description: Exchange WebSocket clients authenticate by subscribing to the `auth` channel with the API secret in a `token` field, or by presenting an auth_token cookie header on connect.
  in: message
  name: WebSocket auth channel
  parameter: token
  sources:
  - https://exchange.blockchain.com/api/
  type: apiKey
slug: blockchain.com-authentication
source_filename: blockchain.com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/blockchain.com-exchange-openapi.yml, openapi/blockchain.com-pay-partner-api-openapi.yml\ndocs: >-\n  https://api.blockchain.com/v3/,\n  https://docs.blockchain.com/pay/api/partner-api/authentication,\n  https://docs.blockchain.com/oauth-resources\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - bearer token (authorization endpoints not publicly documented)\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Token\n  sources:\n  - openapi/blockchain.com-exchange-openapi.yml\n- name: PublicApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Public-API-Key\n  description: Partner's public API key. Required on all endpoints to identify the partner.\n  sources:\n  - openapi/blockchain.com-pay-partner-api-openapi.yml\n- name: PrivateApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Private-API-Key\n  description: Partner's private API key.\
  \ Required on order endpoints; indicates a server-to-server\n    call.\n  sources:\n  - openapi/blockchain.com-pay-partner-api-openapi.yml\n- name: OAuth2 Bearer\n  type: oauth2\n  in: header\n  parameter: Authorization\n  token_type: bearer\n  resource_server: https://api.blockchain.info/partner-resource-gateway\n  scopes:\n  - read_transactions\n  - read_balance\n  scopes_artifact: scopes/blockchain.com-scopes.yml\n  description: >-\n    OAuth 2.0 resource gateway for reading a consenting user's Blockchain.com\n    custodial wallet transactions and balances. Documented only in prose; no\n    OpenAPI and no RFC 8414 / RFC 9728 discovery document is published.\n  sources:\n  - https://docs.blockchain.com/oauth-resources/oauth-resources.md\n- name: WebSocket auth channel\n  type: apiKey\n  in: message\n  parameter: token\n  description: >-\n    Exchange WebSocket clients authenticate by subscribing to the `auth` channel\n    with the API secret in a `token` field, or by presenting an auth_token\
  \ cookie\n    header on connect.\n  sources:\n  - https://exchange.blockchain.com/api/\nnotes:\n- >-\n  No OpenID Connect, no mutualTLS and no HTTP basic anywhere in the public\n  surface. The blockchain.info Data, Simple Query, Charts and Exchange Rates APIs\n  are entirely unauthenticated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/authentication/blockchain.com-authentication.yml
summary_line: apiKey/oauth2 · 5 schemes
tags:
- cryptocurrency
- bitcoin
- blockchain
- exchange
- trading
- market-data
- payments
- on-ramp
- wallet
- block-explorer
- fintech
- webhooks
---
