---
api_key_in:
- header
- query
api_specs:
- filename: coingecko-crypto-market-data-api-openapi.yml
  format: yaml
  label: CoinGecko Crypto Market Data API
  slug: crypto-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/openapi/coingecko-crypto-market-data-api-openapi.yml
- filename: coingecko-pro-api-openapi.yml
  format: yaml
  label: CoinGecko Pro API
  slug: pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/openapi/coingecko-pro-api-openapi.yml
- filename: coingecko-onchain-dex-api-openapi.yml
  format: yaml
  label: CoinGecko Onchain DEX API
  slug: onchain-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/openapi/coingecko-onchain-dex-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coingecko Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinGecko secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CoinGecko
provider_slug: coingecko
scheme_count: 4
schemes:
- description: CoinGecko Demo API key passed via request header. Obtain a free key from the CoinGecko developer dashboard.
  in: header
  name: demoApiKeyHeader
  parameter: x-cg-demo-api-key
  sources:
  - openapi/coingecko-crypto-market-data-api-openapi.yml
  - openapi/coingecko-onchain-dex-api-openapi.yml
  type: apiKey
- description: CoinGecko Demo API key passed via query string parameter.
  in: query
  name: demoApiKeyQuery
  parameter: x_cg_demo_api_key
  sources:
  - openapi/coingecko-crypto-market-data-api-openapi.yml
  - openapi/coingecko-onchain-dex-api-openapi.yml
  type: apiKey
- description: CoinGecko Pro API key passed via request header.
  in: header
  name: proApiKeyHeader
  parameter: x-cg-pro-api-key
  sources:
  - openapi/coingecko-onchain-dex-api-openapi.yml
  - openapi/coingecko-pro-api-openapi.yml
  type: apiKey
- description: CoinGecko Pro API key passed via query string parameter.
  in: query
  name: proApiKeyQuery
  parameter: x_cg_pro_api_key
  sources:
  - openapi/coingecko-onchain-dex-api-openapi.yml
  - openapi/coingecko-pro-api-openapi.yml
  type: apiKey
slug: coingecko-authentication
source_filename: coingecko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coingecko-crypto-market-data-api-openapi.yml, openapi/coingecko-onchain-dex-api-openapi.yml,\n  openapi/coingecko-pro-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: demoApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-cg-demo-api-key\n  description: CoinGecko Demo API key passed via request header. Obtain a free key from the\n    CoinGecko developer dashboard.\n  sources:\n  - openapi/coingecko-crypto-market-data-api-openapi.yml\n  - openapi/coingecko-onchain-dex-api-openapi.yml\n- name: demoApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: x_cg_demo_api_key\n  description: CoinGecko Demo API key passed via query string parameter.\n  sources:\n  - openapi/coingecko-crypto-market-data-api-openapi.yml\n  - openapi/coingecko-onchain-dex-api-openapi.yml\n- name: proApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-cg-pro-api-key\n  description:\
  \ CoinGecko Pro API key passed via request header.\n  sources:\n  - openapi/coingecko-onchain-dex-api-openapi.yml\n  - openapi/coingecko-pro-api-openapi.yml\n- name: proApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: x_cg_pro_api_key\n  description: CoinGecko Pro API key passed via query string parameter.\n  sources:\n  - openapi/coingecko-onchain-dex-api-openapi.yml\n  - openapi/coingecko-pro-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/authentication/coingecko-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Aggregator
- Blockchain
- Cryptocurrency
- Decentralized Exchanges
- DeFi
- DEX
- Exchanges
- Liquidity Pools
- Market Data
- NFTs
- Onchain Data
- Prices
---
