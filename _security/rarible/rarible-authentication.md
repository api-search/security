---
api_key_in:
- header
api_specs:
- filename: rarible-charts-api-openapi.yml
  format: yaml
  label: Rarible Charts API
  slug: rarible-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-charts-api-openapi.yml
- filename: rarible-collection-leader-board-api-openapi.yml
  format: yaml
  label: Rarible Collection Leader Board API
  slug: rarible-collection-leader-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-collection-leader-board-api-openapi.yml
- filename: rarible-collection-statistics-api-openapi.yml
  format: yaml
  label: Rarible Collection Statistics API
  slug: rarible-collection-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-collection-statistics-api-openapi.yml
- filename: rarible-currencies-and-rates-api-openapi.yml
  format: yaml
  label: Rarible Currencies and rates API
  slug: rarible-currencies-and-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-currencies-and-rates-api-openapi.yml
- filename: rarible-domain-lookup-api-openapi.yml
  format: yaml
  label: Rarible Domain lookup API
  slug: rarible-domain-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-domain-lookup-api-openapi.yml
- filename: rarible-encode-operations-api-openapi.yml
  format: yaml
  label: Rarible Encode operations API
  slug: rarible-encode-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-encode-operations-api-openapi.yml
- filename: rarible-indexer-blocks-api-openapi.yml
  format: yaml
  label: Rarible Indexer blocks API
  slug: rarible-indexer-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-indexer-blocks-api-openapi.yml
- filename: rarible-nft-activities-api-openapi.yml
  format: yaml
  label: Rarible NFT Activities API
  slug: rarible-nft-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-activities-api-openapi.yml
- filename: rarible-nft-collections-api-openapi.yml
  format: yaml
  label: Rarible NFT Collections API
  slug: rarible-nft-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-collections-api-openapi.yml
- filename: rarible-nft-data-and-historical-statistics-api-openapi.yml
  format: yaml
  label: Rarible NFT Data and Historical Statistics API
  slug: rarible-nft-data-and-historical-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-data-and-historical-statistics-api-openapi.yml
- filename: rarible-nft-items-api-openapi.yml
  format: yaml
  label: Rarible NFT Items API
  slug: rarible-nft-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-items-api-openapi.yml
- filename: rarible-nft-ownerships-api-openapi.yml
  format: yaml
  label: Rarible NFT Ownerships API
  slug: rarible-nft-ownerships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-ownerships-api-openapi.yml
- filename: rarible-nft-sales-api-openapi.yml
  format: yaml
  label: Rarible NFT Sales API
  slug: rarible-nft-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-sales-api-openapi.yml
- filename: rarible-points-api-openapi.yml
  format: yaml
  label: Rarible Points API
  slug: rarible-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-points-api-openapi.yml
- filename: rarible-reconciliation-api-openapi.yml
  format: yaml
  label: Rarible Reconciliation API
  slug: rarible-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-reconciliation-api-openapi.yml
- filename: rarible-search-api-api-openapi.yml
  format: yaml
  label: Rarible Search API API
  slug: rarible-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-search-api-api-openapi.yml
- filename: rarible-signature-operations-api-openapi.yml
  format: yaml
  label: Rarible Signature operations API
  slug: rarible-signature-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-signature-operations-api-openapi.yml
- filename: rarible-user-balances-api-openapi.yml
  format: yaml
  label: Rarible User balances API
  slug: rarible-user-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-user-balances-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rarible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rarible secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rarible
provider_slug: rarible
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/openapi.yaml
  type: apiKey
slug: rarible-authentication
source_filename: rarible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/authentication/rarible-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NFT
- Non-Fungible Tokens
- Marketplace
- Aggregator
- Multichain
- Ethereum
- Polygon
- Arbitrum
- Flow
- Web3
- Blockchain
- Collection
- Order Book
- Trading
- Indexer
---
