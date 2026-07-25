---
api_key_in:
- header
- query
api_specs:
- filename: footprint-chain-api-openapi.yml
  format: yaml
  label: Footprint Analytics Chain API
  slug: footprint-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-chain-api-openapi.yml
- filename: footprint-defi-api-openapi.yml
  format: yaml
  label: Footprint Analytics DeFi API
  slug: footprint-defi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-defi-api-openapi.yml
- filename: footprint-events-api-openapi.yml
  format: yaml
  label: Footprint Analytics Events API
  slug: footprint-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-events-api-openapi.yml
- filename: footprint-gamefi-api-openapi.yml
  format: yaml
  label: Footprint Analytics GameFi API
  slug: footprint-gamefi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-gamefi-api-openapi.yml
- filename: footprint-nft-api-openapi.yml
  format: yaml
  label: Footprint Analytics NFT API
  slug: footprint-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-nft-api-openapi.yml
- filename: footprint-query-api-openapi.yml
  format: yaml
  label: Footprint Analytics Query API
  slug: footprint-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-query-api-openapi.yml
- filename: footprint-token-api-openapi.yml
  format: yaml
  label: Footprint Analytics Token API
  slug: footprint-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-token-api-openapi.yml
- filename: footprint-wallet-api-openapi.yml
  format: yaml
  label: Footprint Analytics Wallet API
  slug: footprint-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/footprint-wallet-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Footprint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Footprint Analytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Footprint Analytics
provider_slug: footprint
scheme_count: 2
schemes:
- description: Footprint Analytics API key passed as a request header
  in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: Footprint Analytics API key passed as a query parameter
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: footprint-authentication
source_filename: footprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Footprint Analytics API key passed as a request header\n  sources:\n  - openapi/openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Footprint Analytics API key passed as a query parameter\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/authentication/footprint-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Blockchain
- DeFi
- NFT
- GameFi
- Token Analytics
- On-Chain Data
- Web3
- Crypto
---
