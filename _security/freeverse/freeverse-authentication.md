---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Freeverse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freeverse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freeverse
provider_slug: freeverse
scheme_count: 1
schemes:
- applies_to: write mutations
  in: header
  key_binding: Each key is associated with a web3 address that holds LAOS tokens, POLs and ETH used to pay gas for minting/evolving. Testnet keys are pre-funded.
  name: apiKeyHeader
  obtain: Contact info@laosnetwork.io / the LAOS Foundation to request a private API key.
  parameter_name: x-api-key
  sources:
  - graphql/freeverse-laos-client-api-schema.graphql
  type: apiKey
slug: freeverse-authentication
source_filename: freeverse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.laosnetwork.io/api/write-queries/GettingStarted\ndocs: https://docs.laosnetwork.io/api/introduction\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Read-only GraphQL queries (AllCollectionAssets, Inventory, AssetHistory,\n    LAOSCollection, token/tokens/transfers/tokenHistory) require NO authentication.\n    Write mutations (createCollection, mint/mintAsync, evolve/evolveBatch,\n    broadcast) require an API key issued by the LAOS Foundation.\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to: write mutations\n  obtain: Contact info@laosnetwork.io / the LAOS Foundation to request a private API key.\n  key_binding: >-\n    Each key is associated with a web3 address that holds LAOS tokens, POLs and\n    ETH used to pay gas for minting/evolving. Testnet keys are pre-funded.\n  sources: [graphql/freeverse-laos-client-api-schema.graphql]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeverse/refs/heads/main/authentication/freeverse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- NFT
- Web3
- Digital Assets
- Gaming
- GraphQL
- Polkadot
- Ethereum
- Tokenization
---
