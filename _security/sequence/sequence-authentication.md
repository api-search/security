---
api_key_in:
- header
api_specs:
- filename: sequence-indexer.json
  format: json
  label: Sequence Indexer API
  slug: sequence-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-indexer.json
- filename: sequence-metadata.json
  format: json
  label: Sequence Metadata API
  slug: sequence-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-metadata.json
- filename: sequence-marketplace.json
  format: json
  label: Sequence Marketplace API
  slug: sequence-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-marketplace.json
- filename: sequence-transactions.json
  format: json
  label: Sequence Transactions (Relayer) API
  slug: sequence-transactions-relayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-transactions.json
- filename: sequence-analytics.json
  format: json
  label: Sequence Analytics API
  slug: sequence-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-analytics.json
- filename: sequence-builder.json
  format: json
  label: Sequence Builder API
  slug: sequence-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-builder.json
- filename: sequence-infrastructure.json
  format: json
  label: Sequence API (Infrastructure)
  slug: sequence-api-infrastructure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-infrastructure.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sequence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sequence secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sequence
provider_slug: sequence
scheme_count: 2
schemes:
- description: 'Public project access key for authenticating requests obtained on Sequence Builder. Example Test Key: AQAAAAAAAEGvyZiWA9FMslYeG_yayXaHnSI'
  in: header
  name: ApiKeyAuth
  parameter: X-Access-Key
  sources:
  - openapi/sequence-builder.json
  - openapi/sequence-indexer.json
  - openapi/sequence-infrastructure.json
  - openapi/sequence-marketplace.json
  - openapi/sequence-metadata.json
  - openapi/sequence-transactions.json
  type: apiKey
- bearerFormat: JWT
  description: Secret JWT token for authenticating requests obtained from Sequence Builder - should not be exposed publicly.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sequence-builder.json
  - openapi/sequence-indexer.json
  - openapi/sequence-infrastructure.json
  - openapi/sequence-metadata.json
  - openapi/sequence-transactions.json
  type: http
slug: sequence-authentication
source_filename: sequence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sequence-builder.json, openapi/sequence-indexer.json, openapi/sequence-infrastructure.json,\n  openapi/sequence-marketplace.json, openapi/sequence-metadata.json, openapi/sequence-transactions.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Access-Key\n  description: 'Public project access key for authenticating requests obtained on Sequence Builder.\n    Example Test Key: AQAAAAAAAEGvyZiWA9FMslYeG_yayXaHnSI'\n  sources:\n  - openapi/sequence-builder.json\n  - openapi/sequence-indexer.json\n  - openapi/sequence-infrastructure.json\n  - openapi/sequence-marketplace.json\n  - openapi/sequence-metadata.json\n  - openapi/sequence-transactions.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Secret JWT token for authenticating requests obtained from Sequence Builder -\n    should\
  \ not be exposed publicly.\n  sources:\n  - openapi/sequence-builder.json\n  - openapi/sequence-indexer.json\n  - openapi/sequence-infrastructure.json\n  - openapi/sequence-metadata.json\n  - openapi/sequence-transactions.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/authentication/sequence-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Web3
- Blockchain
- Wallets
- Payments
- Crypto
- Indexer
- NFT
- Developer Platform
- Gaming
---
