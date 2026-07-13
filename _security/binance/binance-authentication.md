---
api_key_in:
- header
- query
api_specs:
- filename: binance-spot-trading-openapi.yml
  format: yaml
  label: Binance Spot Trading API
  slug: spot-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-spot-trading-openapi.yml
- filename: binance-spot-websocket-api-asyncapi.yml
  format: yaml
  label: Binance Spot WebSocket API
  slug: spot-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/asyncapi/binance-spot-websocket-api-asyncapi.yml
- filename: binance-spot-websocket-streams-asyncapi.yml
  format: yaml
  label: Binance Spot WebSocket Streams
  slug: spot-websocket-streams
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/asyncapi/binance-spot-websocket-streams-asyncapi.yml
- filename: binance-usds-margined-futures-openapi.yml
  format: yaml
  label: Binance USD-S Margined Futures API
  slug: usds-margined-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-usds-margined-futures-openapi.yml
- filename: binance-coin-margined-futures-openapi.yml
  format: yaml
  label: Binance COIN-M Futures API
  slug: coin-margined-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-coin-margined-futures-openapi.yml
- filename: binance-european-options-openapi.yml
  format: yaml
  label: Binance European Options API
  slug: european-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-european-options-openapi.yml
- filename: binance-portfolio-margin-openapi.yml
  format: yaml
  label: Binance Portfolio Margin API
  slug: portfolio-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-portfolio-margin-openapi.yml
- filename: binance-margin-trading-openapi.yml
  format: yaml
  label: Binance Margin Trading API
  slug: margin-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-margin-trading-openapi.yml
- filename: binance-wallet-openapi.yml
  format: yaml
  label: Binance Wallet API
  slug: wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-wallet-openapi.yml
- filename: binance-sub-account-openapi.yml
  format: yaml
  label: Binance Sub-Account API
  slug: sub-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-sub-account-openapi.yml
- filename: binance-simple-earn-openapi.yml
  format: yaml
  label: Binance Simple Earn API
  slug: simple-earn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-simple-earn-openapi.yml
- filename: binance-mining-openapi.yml
  format: yaml
  label: Binance Mining API
  slug: mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-mining-openapi.yml
- filename: binance-copy-trading-openapi.yml
  format: yaml
  label: Binance Copy Trading API
  slug: copy-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-copy-trading-openapi.yml
- filename: binance-convert-openapi.yml
  format: yaml
  label: Binance Convert API
  slug: convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-convert-openapi.yml
- filename: binance-pay-openapi.yml
  format: yaml
  label: Binance Pay API
  slug: pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-pay-openapi.yml
- filename: binance-algo-trading-openapi.yml
  format: yaml
  label: Binance Algo Trading API
  slug: algo-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-algo-trading-openapi.yml
- filename: binance-auto-invest-openapi.yml
  format: yaml
  label: Binance Auto-Invest API
  slug: auto-invest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-auto-invest-openapi.yml
- filename: binance-crypto-loan-openapi.yml
  format: yaml
  label: Binance Crypto Loan API
  slug: crypto-loan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-crypto-loan-openapi.yml
- filename: binance-gift-card-openapi.yml
  format: yaml
  label: Binance Gift Card API
  slug: gift-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-gift-card-openapi.yml
- filename: binance-nft-openapi.yml
  format: yaml
  label: Binance NFT API
  slug: nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-nft-openapi.yml
- filename: binance-fiat-openapi.yml
  format: yaml
  label: Binance Fiat API
  slug: fiat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/openapi/binance-fiat-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Binance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Binance secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Binance
provider_slug: binance
scheme_count: 3
schemes:
- in: header
  name: apiKey
  parameter: X-MBX-APIKEY
  sources:
  - openapi/binance-algo-trading-openapi.yml
  - openapi/binance-auto-invest-openapi.yml
  - openapi/binance-coin-margined-futures-openapi.yml
  - openapi/binance-convert-openapi.yml
  - openapi/binance-copy-trading-openapi.yml
  - openapi/binance-crypto-loan-openapi.yml
  - openapi/binance-european-options-openapi.yml
  - openapi/binance-fiat-openapi.yml
  - openapi/binance-gift-card-openapi.yml
  - openapi/binance-margin-trading-openapi.yml
  - openapi/binance-mining-openapi.yml
  - openapi/binance-nft-openapi.yml
  - openapi/binance-portfolio-margin-openapi.yml
  - openapi/binance-simple-earn-openapi.yml
  - openapi/binance-spot-trading-openapi.yml
  - openapi/binance-sub-account-openapi.yml
  - openapi/binance-usds-margined-futures-openapi.yml
  - openapi/binance-wallet-openapi.yml
  type: apiKey
- in: query
  name: hmacSignature
  parameter: signature
  sources:
  - openapi/binance-algo-trading-openapi.yml
  - openapi/binance-auto-invest-openapi.yml
  - openapi/binance-coin-margined-futures-openapi.yml
  - openapi/binance-convert-openapi.yml
  - openapi/binance-copy-trading-openapi.yml
  - openapi/binance-crypto-loan-openapi.yml
  - openapi/binance-european-options-openapi.yml
  - openapi/binance-fiat-openapi.yml
  - openapi/binance-gift-card-openapi.yml
  - openapi/binance-margin-trading-openapi.yml
  - openapi/binance-mining-openapi.yml
  - openapi/binance-nft-openapi.yml
  - openapi/binance-portfolio-margin-openapi.yml
  - openapi/binance-simple-earn-openapi.yml
  - openapi/binance-spot-trading-openapi.yml
  - openapi/binance-sub-account-openapi.yml
  - openapi/binance-usds-margined-futures-openapi.yml
  - openapi/binance-wallet-openapi.yml
  type: apiKey
- description: Binance Pay API key/certificate serial number.
  in: header
  name: apiKey
  parameter: BinancePay-Certificate-SN
  sources:
  - openapi/binance-pay-openapi.yml
  type: apiKey
slug: binance-authentication
source_filename: binance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/binance-algo-trading-openapi.yml, openapi/binance-auto-invest-openapi.yml, openapi/binance-coin-margined-futures-openapi.yml,\n  openapi/binance-convert-openapi.yml, openapi/binance-copy-trading-openapi.yml, openapi/binance-crypto-loan-openapi.yml,\n  openapi/binance-european-options-openapi.yml, openapi/binance-fiat-openapi.yml, openapi/binance-gift-card-openapi.yml,\n  openapi/binance-margin-trading-openapi.yml, openapi/binance-mining-openapi.yml, openapi/binance-nft-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-MBX-APIKEY\n  sources:\n  - openapi/binance-algo-trading-openapi.yml\n  - openapi/binance-auto-invest-openapi.yml\n  - openapi/binance-coin-margined-futures-openapi.yml\n  - openapi/binance-convert-openapi.yml\n  - openapi/binance-copy-trading-openapi.yml\n  - openapi/binance-crypto-loan-openapi.yml\n\
  \  - openapi/binance-european-options-openapi.yml\n  - openapi/binance-fiat-openapi.yml\n  - openapi/binance-gift-card-openapi.yml\n  - openapi/binance-margin-trading-openapi.yml\n  - openapi/binance-mining-openapi.yml\n  - openapi/binance-nft-openapi.yml\n  - openapi/binance-portfolio-margin-openapi.yml\n  - openapi/binance-simple-earn-openapi.yml\n  - openapi/binance-spot-trading-openapi.yml\n  - openapi/binance-sub-account-openapi.yml\n  - openapi/binance-usds-margined-futures-openapi.yml\n  - openapi/binance-wallet-openapi.yml\n- name: hmacSignature\n  type: apiKey\n  in: query\n  parameter: signature\n  sources:\n  - openapi/binance-algo-trading-openapi.yml\n  - openapi/binance-auto-invest-openapi.yml\n  - openapi/binance-coin-margined-futures-openapi.yml\n  - openapi/binance-convert-openapi.yml\n  - openapi/binance-copy-trading-openapi.yml\n  - openapi/binance-crypto-loan-openapi.yml\n  - openapi/binance-european-options-openapi.yml\n  - openapi/binance-fiat-openapi.yml\n  - openapi/binance-gift-card-openapi.yml\n\
  \  - openapi/binance-margin-trading-openapi.yml\n  - openapi/binance-mining-openapi.yml\n  - openapi/binance-nft-openapi.yml\n  - openapi/binance-portfolio-margin-openapi.yml\n  - openapi/binance-simple-earn-openapi.yml\n  - openapi/binance-spot-trading-openapi.yml\n  - openapi/binance-sub-account-openapi.yml\n  - openapi/binance-usds-margined-futures-openapi.yml\n  - openapi/binance-wallet-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: BinancePay-Certificate-SN\n  description: Binance Pay API key/certificate serial number.\n  sources:\n  - openapi/binance-pay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/authentication/binance-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- DeFi
- Market Data
---
