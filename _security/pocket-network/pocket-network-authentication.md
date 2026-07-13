---
api_key_in:
- path
api_specs:
- filename: pocket-network-path-gateway-api-openapi.yml
  format: yaml
  label: Pocket Network PATH Gateway API
  slug: pocket-network-path-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-path-gateway-api-openapi.yml
- filename: pocket-network-shannon-rpc-api-openapi.yml
  format: yaml
  label: Pocket Network Shannon RPC API
  slug: pocket-network-shannon-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-shannon-rpc-api-openapi.yml
- filename: pocket-network-cometbft-rpc-api-openapi.yml
  format: yaml
  label: Pocket Network CometBFT RPC API
  slug: pocket-network-cometbft-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-cometbft-rpc-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pocket Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pocket Network secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pocket Network
provider_slug: pocket-network
scheme_count: 1
schemes:
- description: Grove portal Application ID embedded in the relay URL.
  in: path
  name: PortalApplicationId
  parameter: appId
  sources:
  - openapi/pocket-network-path-gateway-api-openapi.yml
  type: apiKey
slug: pocket-network-authentication
source_filename: pocket-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pocket-network-path-gateway-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\nschemes:\n- name: PortalApplicationId\n  type: apiKey\n  in: path\n  parameter: appId\n  description: Grove portal Application ID embedded in the relay URL.\n  sources:\n  - openapi/pocket-network-path-gateway-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/authentication/pocket-network-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Blockchain
- RPC
- Decentralized Infrastructure
- Pocket Network
- Grove
- PATH
- Shannon
- Cosmos
- POKT
---
