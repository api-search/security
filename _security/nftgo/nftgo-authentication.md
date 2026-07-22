---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nftgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: NFTgo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NFTgo
provider_slug: nftgo
scheme_count: 1
schemes:
- description: All NFTgo Developer API requests authenticate with a static API key sent in the X-API-KEY request header. Keys are issued from the developer portal at developer.nftgo.io (or nftgo.io/developers). Usage is metered in Compute Units.
  in: header
  name: apiKeyHeader
  parameter_name: X-API-KEY
  sources:
  - https://docs.nftgo.io/reference/quickstart
  type: apiKey
slug: nftgo-authentication
source_filename: nftgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nftgo.io/reference/quickstart\ndocs: https://docs.nftgo.io/reference/quickstart\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: >-\n    All NFTgo Developer API requests authenticate with a static API key sent in\n    the X-API-KEY request header. Keys are issued from the developer portal at\n    developer.nftgo.io (or nftgo.io/developers). Usage is metered in Compute Units.\n  sources:\n  - https://docs.nftgo.io/reference/quickstart\nkey_management:\n  portal: https://developer.nftgo.io\n  signup: https://nftgo.io/developers\n  dealer_key_provisioning: >-\n    Dealers can mint scoped API keys for their own customers via\n    POST /api/v1/dealer/api_key (see Generate Dealer Key).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nftgo/refs/heads/main/authentication/nftgo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- NFT
- Blockchain
- Web3
- NFT Data
- NFT Analytics
- NFT Trading
- Market Data
- Cryptocurrency
- Ethereum
---
