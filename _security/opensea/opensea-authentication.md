---
api_key_in:
- header
api_specs:
- filename: opensea-api.json
  format: json
  label: OpenSea NFT API
  slug: nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Collection API
  slug: collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Listing API
  slug: listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Offer API
  slug: offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Order API
  slug: order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Drops API
  slug: drops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
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
