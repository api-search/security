---
api_key_in:
- header
- query
api_specs:
- filename: cryptocompare-min-api-openapi.yml
  format: yaml
  label: CryptoCompare min-api (Legacy)
  slug: min-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-min-api-openapi.yml
- filename: cryptocompare-data-api-openapi.yml
  format: yaml
  label: CoinDesk Data API (CCData)
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-data-api-openapi.yml
- filename: cryptocompare-asyncapi.yml
  format: yaml
  label: CryptoCompare Streaming WebSocket
  slug: streamer
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/asyncapi/cryptocompare-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cryptocompare Authentication
name_suffix: Authentication
oauth_flows: []
overview: CryptoCompare secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CryptoCompare
provider_slug: cryptocompare
scheme_count: 2
schemes:
- description: API key supplied as the api_key query parameter.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/cryptocompare-data-api-openapi.yml
  - openapi/cryptocompare-min-api-openapi.yml
  type: apiKey
- description: 'API key supplied as `Authorization: Apikey {apiKey}`.'
  in: header
  name: apiKeyHeader
  parameter: Authorization
  sources:
  - openapi/cryptocompare-data-api-openapi.yml
  - openapi/cryptocompare-min-api-openapi.yml
  type: apiKey
slug: cryptocompare-authentication
source_filename: cryptocompare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cryptocompare-data-api-openapi.yml, openapi/cryptocompare-min-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key supplied as the api_key query parameter.\n  sources:\n  - openapi/cryptocompare-data-api-openapi.yml\n  - openapi/cryptocompare-min-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key supplied as `Authorization: Apikey {apiKey}`.'\n  sources:\n  - openapi/cryptocompare-data-api-openapi.yml\n  - openapi/cryptocompare-min-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/authentication/cryptocompare-authentication.yml
summary_line: apiKey · 2 schemes
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
