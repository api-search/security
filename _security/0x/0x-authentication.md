---
api_key_in:
- header
api_specs:
- filename: 0x-api.yaml
  format: yaml
  label: 0x Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Gasless API
  slug: gasless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-cross-chain.yaml
  format: yaml
  label: 0x Cross-Chain API
  slug: cross-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-cross-chain.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Trade Analytics API
  slug: trade-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Sources API
  slug: sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 0X Authentication
name_suffix: Authentication
oauth_flows: []
overview: 0x secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 0x
provider_slug: 0x
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: 0x-api-key
  sources:
  - openapi/0x-api.yaml
  - openapi/0x-cross-chain.yaml
  type: apiKey
slug: 0x-authentication
source_filename: 0x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/0x-api.yaml, openapi/0x-cross-chain.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: 0x-api-key\n  sources:\n  - openapi/0x-api.yaml\n  - openapi/0x-cross-chain.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/authentication/0x-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- DeFi
- DEX Aggregator
- Swap
- Gasless
- Cross-Chain
- Permit2
- Liquidity
- Trade Analytics
- Web3
- Settlement
- Smart Contracts
---
