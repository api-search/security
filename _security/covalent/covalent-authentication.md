---
api_key_in: []
api_specs:
- filename: covalent-abi-api-openapi.yml
  format: yaml
  label: Covalent ABI API
  slug: covalent-abi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-abi-api-openapi.yml
- filename: covalent-balances-api-openapi.yml
  format: yaml
  label: Covalent Balances API
  slug: covalent-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-balances-api-openapi.yml
- filename: covalent-base-api-openapi.yml
  format: yaml
  label: Covalent Base API
  slug: covalent-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-base-api-openapi.yml
- filename: covalent-bitcoin-api-openapi.yml
  format: yaml
  label: Covalent Bitcoin API
  slug: covalent-bitcoin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-bitcoin-api-openapi.yml
- filename: covalent-cross-chain-api-openapi.yml
  format: yaml
  label: Covalent Cross-Chain API
  slug: covalent-cross-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-cross-chain-api-openapi.yml
- filename: covalent-data-api-openapi.yml
  format: yaml
  label: Covalent Data API
  slug: covalent-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-data-api-openapi.yml
- filename: covalent-destinations-api-openapi.yml
  format: yaml
  label: Covalent Destinations API
  slug: covalent-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-destinations-api-openapi.yml
- filename: covalent-discovery-api-openapi.yml
  format: yaml
  label: Covalent Discovery API
  slug: covalent-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-discovery-api-openapi.yml
- filename: covalent-graphql-api-openapi.yml
  format: yaml
  label: Covalent GraphQL API
  slug: covalent-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-graphql-api-openapi.yml
- filename: covalent-info-api-openapi.yml
  format: yaml
  label: Covalent Info API
  slug: covalent-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-info-api-openapi.yml
- filename: covalent-nft-api-openapi.yml
  format: yaml
  label: Covalent NFT API
  slug: covalent-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-nft-api-openapi.yml
- filename: covalent-pipelines-api-openapi.yml
  format: yaml
  label: Covalent Pipelines API
  slug: covalent-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-pipelines-api-openapi.yml
- filename: covalent-pricing-api-openapi.yml
  format: yaml
  label: Covalent Pricing API
  slug: covalent-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-pricing-api-openapi.yml
- filename: covalent-security-api-openapi.yml
  format: yaml
  label: Covalent Security API
  slug: covalent-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-security-api-openapi.yml
- filename: covalent-transactions-api-openapi.yml
  format: yaml
  label: Covalent Transactions API
  slug: covalent-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-transactions-api-openapi.yml
- filename: covalent-transforms-api-openapi.yml
  format: yaml
  label: Covalent Transforms API
  slug: covalent-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-transforms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Covalent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Covalent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Covalent
provider_slug: covalent
scheme_count: 1
schemes:
- description: 'GoldRush API key, sent as `Authorization: Bearer <key>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/covalent-foundational-api-openapi.yml
  - openapi/covalent-hyperliquid-info-api-openapi.yml
  - openapi/covalent-pipeline-api-openapi.yml
  - openapi/covalent-streaming-api-openapi.yml
  - openapi/covalent-x402-api-openapi.yml
  type: http
slug: covalent-authentication
source_filename: covalent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/covalent-foundational-api-openapi.yml, openapi/covalent-hyperliquid-info-api-openapi.yml,\n  openapi/covalent-pipeline-api-openapi.yml, openapi/covalent-streaming-api-openapi.yml, openapi/covalent-x402-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'GoldRush API key, sent as `Authorization: Bearer <key>`.'\n  sources:\n  - openapi/covalent-foundational-api-openapi.yml\n  - openapi/covalent-hyperliquid-info-api-openapi.yml\n  - openapi/covalent-pipeline-api-openapi.yml\n  - openapi/covalent-streaming-api-openapi.yml\n  - openapi/covalent-x402-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/authentication/covalent-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Web3
- Multi-Chain
- Data Infrastructure
- Crypto
- DeFi
- NFT
- Hyperliquid
- GoldRush
- AI Agents
---
