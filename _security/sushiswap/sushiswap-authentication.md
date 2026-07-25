---
api_key_in:
- header
api_specs:
- filename: sushiswap-deposit-api-openapi.yml
  format: yaml
  label: SushiSwap Deposit API
  slug: sushiswap-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/openapi/sushiswap-deposit-api-openapi.yml
- filename: sushiswap-liquidity-providers-api-openapi.yml
  format: yaml
  label: SushiSwap liquidity-providers API
  slug: sushiswap-liquidity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/openapi/sushiswap-liquidity-providers-api-openapi.yml
- filename: sushiswap-pool-api-openapi.yml
  format: yaml
  label: SushiSwap Pool API
  slug: sushiswap-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/openapi/sushiswap-pool-api-openapi.yml
- filename: sushiswap-price-api-openapi.yml
  format: yaml
  label: SushiSwap price API
  slug: sushiswap-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/openapi/sushiswap-price-api-openapi.yml
- filename: sushiswap-quote-api-openapi.yml
  format: yaml
  label: SushiSwap Quote API
  slug: sushiswap-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/openapi/sushiswap-quote-api-openapi.yml
- filename: sushiswap-swap-api-openapi.yml
  format: yaml
  label: SushiSwap swap API
  slug: sushiswap-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/openapi/sushiswap-swap-api-openapi.yml
- filename: sushiswap-token-api-openapi.yml
  format: yaml
  label: SushiSwap token API
  slug: sushiswap-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/openapi/sushiswap-token-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sushiswap Authentication
name_suffix: Authentication
oauth_flows: []
overview: SushiSwap secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SushiSwap
provider_slug: sushiswap
scheme_count: 1
schemes:
- description: API key required for all endpoints. In order to prevent abuse on the API we implement rate limits on the requests, to overcome these limits as an aggregator get in contact with the [support team](mailto:aggregators@shipyardsoftware.org) to get API credentials.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/blade-v2-openapi.json
  type: apiKey
slug: sushiswap-authentication
source_filename: sushiswap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blade-v2-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key required for all endpoints. In order to prevent abuse on the API we implement\n    rate limits on the requests, to overcome these limits as an aggregator get in contact with\n    the [support team](mailto:aggregators@shipyardsoftware.org) to get API credentials.\n  sources:\n  - openapi/blade-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/authentication/sushiswap-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DeFi
- Decentralized Exchange
- DEX
- Cryptocurrency
- Web3
- Blockchain
- Multi-Chain
- Liquidity
- Swap
- Token Pricing
---
