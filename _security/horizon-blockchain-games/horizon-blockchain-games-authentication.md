---
api_key_in:
- header
api_specs:
- filename: horizon-blockchain-games-indexer-openapi-original.json
  format: json
  label: Sequence Indexer API
  slug: sequence-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-indexer-openapi-original.json
- filename: horizon-blockchain-games-metadata-openapi-original.json
  format: json
  label: Sequence Metadata API
  slug: sequence-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-metadata-openapi-original.json
- filename: horizon-blockchain-games-marketplace-openapi-original.json
  format: json
  label: Sequence Marketplace API
  slug: sequence-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-marketplace-openapi-original.json
- filename: horizon-blockchain-games-transactions-openapi-original.json
  format: json
  label: Sequence Transactions (Relayer) API
  slug: sequence-transactions-relayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-transactions-openapi-original.json
- filename: horizon-blockchain-games-analytics-openapi-original.json
  format: json
  label: Sequence Analytics API
  slug: sequence-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-analytics-openapi-original.json
- filename: horizon-blockchain-games-builder-openapi-original.json
  format: json
  label: Sequence Builder API
  slug: sequence-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-builder-openapi-original.json
- filename: horizon-blockchain-games-infrastructure-openapi-original.json
  format: json
  label: Sequence API (Infrastructure)
  slug: sequence-api-infrastructure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-infrastructure-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Horizon Blockchain Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: Horizon Blockchain Games secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Horizon Blockchain Games
provider_slug: horizon-blockchain-games
scheme_count: 2
schemes:
- description: 'Public project access key for authenticating requests obtained on Sequence Builder. Example Test Key: AQAAAAAAAEGvyZiWA9FMslYeG_yayXaHnSI'
  in: header
  name: ApiKeyAuth
  parameter: X-Access-Key
  sources:
  - openapi/horizon-blockchain-games-builder-openapi-original.json
  - openapi/horizon-blockchain-games-indexer-openapi-original.json
  - openapi/horizon-blockchain-games-infrastructure-openapi-original.json
  - openapi/horizon-blockchain-games-marketplace-openapi-original.json
  - openapi/horizon-blockchain-games-metadata-openapi-original.json
  - openapi/horizon-blockchain-games-transactions-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  description: Secret JWT token for authenticating requests obtained from Sequence Builder - should not be exposed publicly.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/horizon-blockchain-games-builder-openapi-original.json
  - openapi/horizon-blockchain-games-indexer-openapi-original.json
  - openapi/horizon-blockchain-games-infrastructure-openapi-original.json
  - openapi/horizon-blockchain-games-metadata-openapi-original.json
  - openapi/horizon-blockchain-games-transactions-openapi-original.json
  type: http
slug: horizon-blockchain-games-authentication
source_filename: horizon-blockchain-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/horizon-blockchain-games-builder-openapi-original.json, openapi/horizon-blockchain-games-indexer-openapi-original.json,\n  openapi/horizon-blockchain-games-infrastructure-openapi-original.json, openapi/horizon-blockchain-games-marketplace-openapi-original.json,\n  openapi/horizon-blockchain-games-metadata-openapi-original.json, openapi/horizon-blockchain-games-transactions-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Access-Key\n  description: 'Public project access key for authenticating requests obtained on Sequence Builder.\n    Example Test Key: AQAAAAAAAEGvyZiWA9FMslYeG_yayXaHnSI'\n  sources:\n  - openapi/horizon-blockchain-games-builder-openapi-original.json\n  - openapi/horizon-blockchain-games-indexer-openapi-original.json\n  - openapi/horizon-blockchain-games-infrastructure-openapi-original.json\n\
  \  - openapi/horizon-blockchain-games-marketplace-openapi-original.json\n  - openapi/horizon-blockchain-games-metadata-openapi-original.json\n  - openapi/horizon-blockchain-games-transactions-openapi-original.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Secret JWT token for authenticating requests obtained from Sequence Builder -\n    should not be exposed publicly.\n  sources:\n  - openapi/horizon-blockchain-games-builder-openapi-original.json\n  - openapi/horizon-blockchain-games-indexer-openapi-original.json\n  - openapi/horizon-blockchain-games-infrastructure-openapi-original.json\n  - openapi/horizon-blockchain-games-metadata-openapi-original.json\n  - openapi/horizon-blockchain-games-transactions-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/authentication/horizon-blockchain-games-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Consumer
- Blockchain
- Web3
- Gaming
- NFT
- Wallet
- Cryptocurrency
- Smart Contracts
- Marketplace
- Developer Tools
- Ethereum
---
