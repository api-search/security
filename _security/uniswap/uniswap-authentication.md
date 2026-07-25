---
api_key_in:
- header
api_specs:
- filename: uniswap-approval-api-openapi.yml
  format: yaml
  label: Uniswap Approval API
  slug: uniswap-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-approval-api-openapi.yml
- filename: uniswap-limitorderquote-api-openapi.yml
  format: yaml
  label: Uniswap LimitOrderQuote API
  slug: uniswap-limitorderquote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-limitorderquote-api-openapi.yml
- filename: uniswap-liquidity-api-openapi.yml
  format: yaml
  label: Uniswap Liquidity API
  slug: uniswap-liquidity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-liquidity-api-openapi.yml
- filename: uniswap-order-api-openapi.yml
  format: yaml
  label: Uniswap Order API
  slug: uniswap-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-order-api-openapi.yml
- filename: uniswap-plan-api-openapi.yml
  format: yaml
  label: Uniswap Plan API
  slug: uniswap-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-plan-api-openapi.yml
- filename: uniswap-quote-api-openapi.yml
  format: yaml
  label: Uniswap Quote API
  slug: uniswap-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-quote-api-openapi.yml
- filename: uniswap-send-api-openapi.yml
  format: yaml
  label: Uniswap Send API
  slug: uniswap-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-send-api-openapi.yml
- filename: uniswap-swap-api-openapi.yml
  format: yaml
  label: Uniswap Swap API
  slug: uniswap-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-swap-api-openapi.yml
- filename: uniswap-swappabletokens-api-openapi.yml
  format: yaml
  label: Uniswap SwappableTokens API
  slug: uniswap-swappabletokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-swappabletokens-api-openapi.yml
- filename: uniswap-wallet-api-openapi.yml
  format: yaml
  label: Uniswap Wallet API
  slug: uniswap-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-wallet-api-openapi.yml
- filename: uniswap-walletcheckdelegation-api-openapi.yml
  format: yaml
  label: Uniswap WalletCheckDelegation API
  slug: uniswap-walletcheckdelegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-walletcheckdelegation-api-openapi.yml
- filename: uniswap-walletencode7702-api-openapi.yml
  format: yaml
  label: Uniswap WalletEncode7702 API
  slug: uniswap-walletencode7702-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-walletencode7702-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uniswap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uniswap secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uniswap
provider_slug: uniswap
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/uniswap-trading-openapi.json
  - openapi/uniswap-trading-openapi.yaml
  type: apiKey
slug: uniswap-authentication
source_filename: uniswap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uniswap-trading-openapi.json, openapi/uniswap-trading-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/uniswap-trading-openapi.json\n  - openapi/uniswap-trading-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/authentication/uniswap-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cryptocurrency
- DeFi
- Decentralized Exchange
- Liquidity
- Swaps
---
