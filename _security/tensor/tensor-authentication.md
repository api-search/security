---
api_key_in:
- header
api_specs:
- filename: tensor-websocket-api-asyncapi.yml
  format: yaml
  label: Tensor WebSocket API
  slug: tensor-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/asyncapi/tensor-websocket-api-asyncapi.yml
- filename: tensor-bids-api-openapi.yml
  format: yaml
  label: Tensor Bids API
  slug: tensor-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-bids-api-openapi.yml
- filename: tensor-collections-api-openapi.yml
  format: yaml
  label: Tensor Collections API
  slug: tensor-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-collections-api-openapi.yml
- filename: tensor-escrow-api-openapi.yml
  format: yaml
  label: Tensor Escrow API
  slug: tensor-escrow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-escrow-api-openapi.yml
- filename: tensor-listings-api-openapi.yml
  format: yaml
  label: Tensor Listings API
  slug: tensor-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-listings-api-openapi.yml
- filename: tensor-nfts-api-openapi.yml
  format: yaml
  label: Tensor NFTs API
  slug: tensor-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-nfts-api-openapi.yml
- filename: tensor-pools-api-openapi.yml
  format: yaml
  label: Tensor Pools API
  slug: tensor-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-pools-api-openapi.yml
- filename: tensor-user-api-openapi.yml
  format: yaml
  label: Tensor User API
  slug: tensor-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-user-api-openapi.yml
- filename: tensor-utility-api-openapi.yml
  format: yaml
  label: Tensor Utility API
  slug: tensor-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-utility-api-openapi.yml
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
