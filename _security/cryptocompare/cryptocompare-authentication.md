---
api_key_in:
- header
- query
api_specs:
- filename: cryptocompare-asyncapi.yml
  format: yaml
  label: CryptoCompare Streaming WebSocket
  slug: streamer
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/asyncapi/cryptocompare-asyncapi.yml
- filename: cryptocompare-asset-api-openapi.yml
  format: yaml
  label: CryptoCompare Asset API
  slug: cryptocompare-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-asset-api-openapi.yml
- filename: cryptocompare-blockchain-api-openapi.yml
  format: yaml
  label: CryptoCompare Blockchain API
  slug: cryptocompare-blockchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-blockchain-api-openapi.yml
- filename: cryptocompare-coins-api-openapi.yml
  format: yaml
  label: CryptoCompare Coins API
  slug: cryptocompare-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-coins-api-openapi.yml
- filename: cryptocompare-exchanges-api-openapi.yml
  format: yaml
  label: CryptoCompare Exchanges API
  slug: cryptocompare-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-exchanges-api-openapi.yml
- filename: cryptocompare-futures-api-openapi.yml
  format: yaml
  label: CryptoCompare Futures API
  slug: cryptocompare-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-futures-api-openapi.yml
- filename: cryptocompare-historical-api-openapi.yml
  format: yaml
  label: CryptoCompare Historical API
  slug: cryptocompare-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-historical-api-openapi.yml
- filename: cryptocompare-index-api-openapi.yml
  format: yaml
  label: CryptoCompare Index API
  slug: cryptocompare-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-index-api-openapi.yml
- filename: cryptocompare-news-api-openapi.yml
  format: yaml
  label: CryptoCompare News API
  slug: cryptocompare-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-news-api-openapi.yml
- filename: cryptocompare-on-chain-api-openapi.yml
  format: yaml
  label: CryptoCompare On-Chain API
  slug: cryptocompare-on-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-on-chain-api-openapi.yml
- filename: cryptocompare-options-api-openapi.yml
  format: yaml
  label: CryptoCompare Options API
  slug: cryptocompare-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-options-api-openapi.yml
- filename: cryptocompare-order-book-api-openapi.yml
  format: yaml
  label: CryptoCompare Order Book API
  slug: cryptocompare-order-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-order-book-api-openapi.yml
- filename: cryptocompare-overview-api-openapi.yml
  format: yaml
  label: CryptoCompare Overview API
  slug: cryptocompare-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-overview-api-openapi.yml
- filename: cryptocompare-price-api-openapi.yml
  format: yaml
  label: CryptoCompare Price API
  slug: cryptocompare-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-price-api-openapi.yml
- filename: cryptocompare-social-api-openapi.yml
  format: yaml
  label: CryptoCompare Social API
  slug: cryptocompare-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-social-api-openapi.yml
- filename: cryptocompare-spot-api-openapi.yml
  format: yaml
  label: CryptoCompare Spot API
  slug: cryptocompare-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-spot-api-openapi.yml
- filename: cryptocompare-top-lists-api-openapi.yml
  format: yaml
  label: CryptoCompare Top Lists API
  slug: cryptocompare-top-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-top-lists-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cryptocompare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CryptoCompare secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CryptoCompare
provider_slug: cryptocompare
scheme_count: 3
schemes:
- description: API key supplied as the api_key query parameter.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/_original/cryptocompare-data-api-openapi.yml
  - openapi/_original/cryptocompare-min-api-openapi.yml
  type: apiKey
- description: 'API key supplied as `Authorization: Apikey {apiKey}`.'
  in: header
  name: apiKeyHeader
  parameter: Authorization
  sources:
  - openapi/_original/cryptocompare-data-api-openapi.yml
  - openapi/_original/cryptocompare-min-api-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization code + PKCE (S256) with dynamic client registration, used only by the official MCP server at https://mcp.coindesk.com/mcp — it wraps the user's CoinDesk Data API key, which is stored encrypted. No scopes (scopes_supported is empty).
  flows:
  - authorizationUrl: https://mcp.coindesk.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.coindesk.com/token
  name: mcpOAuth
  sources:
  - well-known/cryptocompare-oauth-authorization-server.json
  type: oauth2
slug: cryptocompare-authentication
source_filename: cryptocompare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/cryptocompare-*-openapi.yml + https://mcp.coindesk.com/.well-known/oauth-authorization-server + live 401 probes\ndocs: https://developers.coindesk.com/documentation/data-api/introduction\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key supplied as the api_key query parameter.\n  sources:\n  - openapi/_original/cryptocompare-data-api-openapi.yml\n  - openapi/_original/cryptocompare-min-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key supplied as `Authorization: Apikey {apiKey}`.'\n  sources:\n  - openapi/_original/cryptocompare-data-api-openapi.yml\n  - openapi/_original/cryptocompare-min-api-openapi.yml\n- name: mcpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.0\
  \ authorization code + PKCE (S256) with dynamic client registration,\n    used only by the official MCP server at https://mcp.coindesk.com/mcp — it\n    wraps the user's CoinDesk Data API key, which is stored encrypted. No scopes\n    (scopes_supported is empty).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.coindesk.com/authorize\n    tokenUrl: https://mcp.coindesk.com/token\n  sources:\n  - well-known/cryptocompare-oauth-authorization-server.json\nnotes: >-\n  Since 2026-05-21 the free tier is retired: every request without a key under an\n  active subscription returns HTTP 401 with Err.type 2 \"API key required\"\n  (verified live 2026-07-22 on both min-api and data-api). Keys are managed in the\n  developers.coindesk.com dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/authentication/cryptocompare-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Cryptocurrency
- Market Data
- Reference Rates
- News
- Social
- Blockchain
- On-Chain
- Order Book
- Streaming
- Index
---
