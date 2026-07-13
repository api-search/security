---
api_key_in:
- header
api_specs:
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Coin Query API
  slug: iota-coin-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Read API
  slug: iota-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Extended API
  slug: iota-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Governance Read API
  slug: iota-governance-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Move Utils API
  slug: iota-move-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Transaction Builder API
  slug: iota-transaction-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Write API
  slug: iota-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-evm-wasp-openapi.yaml
  format: yaml
  label: IOTA EVM JSON-RPC API
  slug: iota-evm-json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-evm-wasp-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Iota Authentication
name_suffix: Authentication
oauth_flows: []
overview: IOTA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IOTA
provider_slug: iota
scheme_count: 1
schemes:
- description: JWT Token
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/iota-evm-wasp-openapi.yaml
  type: apiKey
slug: iota-authentication
source_filename: iota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iota-evm-wasp-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT Token\n  sources:\n  - openapi/iota-evm-wasp-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/authentication/iota-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Distributed Ledger
- Web3
- DeFi
- Cryptocurrency
- Move
- Tangle
---
