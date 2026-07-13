---
api_key_in:
- header
api_specs:
- filename: tensor-api-openapi.yml
  format: yaml
  label: Tensor API
  slug: tensor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-api-openapi.yml
- filename: tensor-tx-api-openapi.yml
  format: yaml
  label: Tensor Transaction API
  slug: tensor-tx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-tx-api-openapi.yml
- filename: tensor-websocket-api-asyncapi.yml
  format: yaml
  label: Tensor WebSocket API
  slug: tensor-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/asyncapi/tensor-websocket-api-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tensor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tensor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tensor
provider_slug: tensor
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-tensor-api-key
  sources:
  - openapi/tensor-api-openapi.yml
  - openapi/tensor-tx-api-openapi.yml
  type: apiKey
slug: tensor-authentication
source_filename: tensor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tensor-api-openapi.yml, openapi/tensor-tx-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-tensor-api-key\n  sources:\n  - openapi/tensor-api-openapi.yml\n  - openapi/tensor-tx-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/authentication/tensor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NFT
- Marketplace
- Solana
- Blockchain
- Web3
- Cryptocurrency
- Trading
- DAO
- DeFi
- AMM
---
