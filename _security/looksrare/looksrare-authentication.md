---
api_key_in:
- header
api_specs:
- filename: looksrare-openapi.json
  format: json
  label: LooksRare Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looksrare/refs/heads/main/openapi/looksrare-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Looksrare Authentication
name_suffix: Authentication
oauth_flows: []
overview: LooksRare secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LooksRare
provider_slug: looksrare
scheme_count: 1
schemes:
- description: API key required for mainnet write operations (order creation). Not needed for read endpoints or testnet.
  in: header
  name: ApiKeyHeader
  parameter: X-Looks-Api-Key
  sources:
  - openapi/looksrare-openapi.json
  type: apiKey
slug: looksrare-authentication
source_filename: looksrare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/looksrare-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Looks-Api-Key\n  description: API key required for mainnet write operations (order creation). Not needed for\n    read endpoints or testnet.\n  sources:\n  - openapi/looksrare-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looksrare/refs/heads/main/authentication/looksrare-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NFT
- Marketplace
- Ethereum
- Web3
- Orders
- Collections
- Tokens
- Events
- ERC-721
- ERC-1155
- Seaport
- Community
---
