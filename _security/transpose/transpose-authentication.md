---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Transpose Block API
  slug: transpose-block-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose Token API
  slug: transpose-token-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/verified-endpoints/token-api/overview/
- filename: openapi.yaml
  format: yaml
  label: Transpose NFT API
  slug: transpose-nft-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose ENS API
  slug: transpose-ens-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose Token Prices API
  slug: transpose-token-prices-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/verified-endpoints/token-prices-api/overview/
- filename: openapi.yaml
  format: yaml
  label: Transpose SQL Analytics API
  slug: transpose-sql-analytics-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Transpose Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transpose secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transpose
provider_slug: transpose
scheme_count: 1
schemes:
- description: API key obtained from your Transpose team dashboard.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: transpose-authentication
source_filename: transpose-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key obtained from your Transpose team dashboard.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transpose/refs/heads/main/authentication/transpose-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- NFT
- Cryptocurrency
- Web3
- Ethereum
- Token Transfers
- Smart Contracts
- Historical Data
- DeFi
- DEX
---
