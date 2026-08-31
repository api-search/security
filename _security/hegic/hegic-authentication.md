---
api_key_in:
- query
api_specs:
- filename: hegic-accounts-api-openapi.yml
  format: yaml
  label: Hegic Accounts API
  slug: hegic-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/openapi/hegic-accounts-api-openapi.yml
- filename: hegic-contracts-api-openapi.yml
  format: yaml
  label: Hegic Contracts API
  slug: hegic-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/openapi/hegic-contracts-api-openapi.yml
- filename: hegic-fees-api-openapi.yml
  format: yaml
  label: Hegic Fees API
  slug: hegic-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/openapi/hegic-fees-api-openapi.yml
- filename: hegic-options-api-openapi.yml
  format: yaml
  label: Hegic Options API
  slug: hegic-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/openapi/hegic-options-api-openapi.yml
- filename: hegic-prices-api-openapi.yml
  format: yaml
  label: Hegic Prices API
  slug: hegic-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/openapi/hegic-prices-api-openapi.yml
- filename: hegic-tokens-api-openapi.yml
  format: yaml
  label: Hegic Tokens API
  slug: hegic-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/openapi/hegic-tokens-api-openapi.yml
- filename: hegic-tvl-api-openapi.yml
  format: yaml
  label: Hegic TVL API
  slug: hegic-tvl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/openapi/hegic-tvl-api-openapi.yml
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
