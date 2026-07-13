---
api_key_in:
- query
api_specs:
- filename: api-docs.defillama.com
  format: yaml
  label: DefiLlama Hegic Protocol API
  slug: defillama-hegic-protocol-api
  spec_type: OpenAPI
  url: https://api-docs.defillama.com
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hegic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hegic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hegic
provider_slug: hegic
scheme_count: 1
schemes:
- in: query
  name: ApiKeyQuery
  parameter: apikey
  sources:
  - openapi/arbiscan-token.yml
  type: apiKey
slug: hegic-authentication
source_filename: hegic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arbiscan-token.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/arbiscan-token.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/authentication/hegic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DeFi
- Options Trading
- On-Chain
- Arbitrum
- Ethereum
- Liquidity Pools
- AMM
- Derivatives
- Web3
---
