---
api_key_in:
- header
api_specs:
- filename: alchemy-asyncapi.yml
  format: yaml
  label: Alchemy Node API (JSON-RPC)
  slug: node-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/asyncapi/alchemy-asyncapi.yml
- filename: alchemy-token-api-openapi.yml
  format: yaml
  label: Alchemy Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/openapi/alchemy-token-api-openapi.yml
- filename: alchemy-transfers-api-openapi.yml
  format: yaml
  label: Alchemy Transfers API
  slug: transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/openapi/alchemy-transfers-api-openapi.yml
- filename: alchemy-gas-manager-api-openapi.yml
  format: yaml
  label: Alchemy Gas Manager API
  slug: gas-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/openapi/alchemy-gas-manager-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alchemy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alchemy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alchemy
provider_slug: alchemy
scheme_count: 2
schemes:
- description: Bearer token for Gas Manager Management API authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alchemy-gas-manager-api-openapi.yml
  type: http
- description: Alchemy API key for RPC endpoint authentication.
  in: header
  name: apiKeyHeader
  parameter: X-Alchemy-Token
  sources:
  - openapi/alchemy-gas-manager-api-openapi.yml
  - openapi/alchemy-token-api-openapi.yml
  - openapi/alchemy-transfers-api-openapi.yml
  type: apiKey
slug: alchemy-authentication
source_filename: alchemy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alchemy-gas-manager-api-openapi.yml, openapi/alchemy-token-api-openapi.yml,\n  openapi/alchemy-transfers-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for Gas Manager Management API authentication.\n  sources:\n  - openapi/alchemy-gas-manager-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Alchemy-Token\n  description: Alchemy API key for RPC endpoint authentication.\n  sources:\n  - openapi/alchemy-gas-manager-api-openapi.yml\n  - openapi/alchemy-token-api-openapi.yml\n  - openapi/alchemy-transfers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/authentication/alchemy-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Web3
- Blockchain
- RPC
- NFT
- Indexing
- Account Abstraction
---
