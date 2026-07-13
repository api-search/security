---
api_key_in:
- header
api_specs:
- filename: blade-v2-openapi.json
  format: json
  label: Sushi Price API
  slug: sushi-price-api
  spec_type: OpenAPI
  url: https://docs.sushi.com/blade-v2-openapi.json
- filename: blade-v2-openapi.json
  format: json
  label: Sushi Quote API
  slug: sushi-quote-api
  spec_type: OpenAPI
  url: https://docs.sushi.com/blade-v2-openapi.json
- filename: blade-v2-openapi.json
  format: json
  label: Sushi Swap API
  slug: sushi-swap-api
  spec_type: OpenAPI
  url: https://docs.sushi.com/blade-v2-openapi.json
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
