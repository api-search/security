---
api_key_in:
- path
api_specs:
- filename: pocket-network-application-api-openapi.yml
  format: yaml
  label: Pocket Network Application API
  slug: pocket-network-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-application-api-openapi.yml
- filename: pocket-network-bank-api-openapi.yml
  format: yaml
  label: Pocket Network Bank API
  slug: pocket-network-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-bank-api-openapi.yml
- filename: pocket-network-blocks-api-openapi.yml
  format: yaml
  label: Pocket Network Blocks API
  slug: pocket-network-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-blocks-api-openapi.yml
- filename: pocket-network-consensus-api-openapi.yml
  format: yaml
  label: Pocket Network Consensus API
  slug: pocket-network-consensus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-consensus-api-openapi.yml
- filename: pocket-network-gateway-api-openapi.yml
  format: yaml
  label: Pocket Network Gateway API
  slug: pocket-network-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-gateway-api-openapi.yml
- filename: pocket-network-health-api-openapi.yml
  format: yaml
  label: Pocket Network Health API
  slug: pocket-network-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-health-api-openapi.yml
- filename: pocket-network-mempool-api-openapi.yml
  format: yaml
  label: Pocket Network Mempool API
  slug: pocket-network-mempool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-mempool-api-openapi.yml
- filename: pocket-network-proof-api-openapi.yml
  format: yaml
  label: Pocket Network Proof API
  slug: pocket-network-proof-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-proof-api-openapi.yml
- filename: pocket-network-relays-api-openapi.yml
  format: yaml
  label: Pocket Network Relays API
  slug: pocket-network-relays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-relays-api-openapi.yml
- filename: pocket-network-service-api-openapi.yml
  format: yaml
  label: Pocket Network Service API
  slug: pocket-network-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-service-api-openapi.yml
- filename: pocket-network-session-api-openapi.yml
  format: yaml
  label: Pocket Network Session API
  slug: pocket-network-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-session-api-openapi.yml
- filename: pocket-network-status-api-openapi.yml
  format: yaml
  label: Pocket Network Status API
  slug: pocket-network-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-status-api-openapi.yml
- filename: pocket-network-supplier-api-openapi.yml
  format: yaml
  label: Pocket Network Supplier API
  slug: pocket-network-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-supplier-api-openapi.yml
- filename: pocket-network-tokenomics-api-openapi.yml
  format: yaml
  label: Pocket Network Tokenomics API
  slug: pocket-network-tokenomics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-tokenomics-api-openapi.yml
- filename: pocket-network-transactions-api-openapi.yml
  format: yaml
  label: Pocket Network Transactions API
  slug: pocket-network-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-transactions-api-openapi.yml
- filename: pocket-network-validators-api-openapi.yml
  format: yaml
  label: Pocket Network Validators API
  slug: pocket-network-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-validators-api-openapi.yml
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
