---
api_key_in:
- header
api_specs:
- filename: opensea-account-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Account Endpoints API
  slug: opensea-account-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-account-endpoints-api-openapi.yml
- filename: opensea-analytics-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Analytics Endpoints API
  slug: opensea-analytics-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-analytics-endpoints-api-openapi.yml
- filename: opensea-auth-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Auth Endpoints API
  slug: opensea-auth-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-auth-endpoints-api-openapi.yml
- filename: opensea-chain-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Chain Endpoints API
  slug: opensea-chain-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-chain-endpoints-api-openapi.yml
- filename: opensea-collection-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Collection Endpoints API
  slug: opensea-collection-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-collection-endpoints-api-openapi.yml
- filename: opensea-contract-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Contract Endpoints API
  slug: opensea-contract-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-contract-endpoints-api-openapi.yml
- filename: opensea-drops-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Drops Endpoints API
  slug: opensea-drops-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-drops-endpoints-api-openapi.yml
- filename: opensea-listing-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Listing Endpoints API
  slug: opensea-listing-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-listing-endpoints-api-openapi.yml
- filename: opensea-nft-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea NFT Endpoints API
  slug: opensea-nft-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-nft-endpoints-api-openapi.yml
- filename: opensea-offer-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Offer Endpoints API
  slug: opensea-offer-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-offer-endpoints-api-openapi.yml
- filename: opensea-order-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Order Endpoints API
  slug: opensea-order-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-order-endpoints-api-openapi.yml
- filename: opensea-search-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Search Endpoints API
  slug: opensea-search-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-search-endpoints-api-openapi.yml
- filename: opensea-swap-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Swap Endpoints API
  slug: opensea-swap-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-swap-endpoints-api-openapi.yml
- filename: opensea-token-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Token Endpoints API
  slug: opensea-token-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-token-endpoints-api-openapi.yml
- filename: opensea-tool-endpoints-beta-api-openapi.yml
  format: yaml
  label: OpenSea Tool Endpoints [Beta] API
  slug: opensea-tool-endpoints-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-tool-endpoints-beta-api-openapi.yml
- filename: opensea-transaction-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Transaction Endpoints API
  slug: opensea-transaction-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-transaction-endpoints-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opensea Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenSea secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenSea
provider_slug: opensea
scheme_count: 1
schemes:
- description: API key required for authentication
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/opensea-api.json
  type: apiKey
slug: opensea-authentication
source_filename: opensea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opensea-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key required for authentication\n  sources:\n  - openapi/opensea-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/authentication/opensea-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NFT
- Marketplace
- Web3
- Blockchain
- Trading
- Digital Assets
---
