---
api_key_in:
- header
api_specs:
- filename: quicknode-asyncapi.yml
  format: yaml
  label: QuickNode Core RPC API
  slug: core-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/asyncapi/quicknode-asyncapi.yml
- filename: quicknode-account-api-openapi.yml
  format: yaml
  label: QuickNode Account API
  slug: quicknode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-account-api-openapi.yml
- filename: quicknode-batch-api-openapi.yml
  format: yaml
  label: QuickNode Batch API
  slug: quicknode-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-batch-api-openapi.yml
- filename: quicknode-database-api-openapi.yml
  format: yaml
  label: QuickNode Database API
  slug: quicknode-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-database-api-openapi.yml
- filename: quicknode-gateway-api-openapi.yml
  format: yaml
  label: QuickNode Gateway API
  slug: quicknode-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-gateway-api-openapi.yml
- filename: quicknode-keys-api-openapi.yml
  format: yaml
  label: QuickNode Keys API
  slug: quicknode-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-keys-api-openapi.yml
- filename: quicknode-logs-api-openapi.yml
  format: yaml
  label: QuickNode Logs API
  slug: quicknode-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-logs-api-openapi.yml
- filename: quicknode-pinning-api-openapi.yml
  format: yaml
  label: QuickNode Pinning API
  slug: quicknode-pinning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-pinning-api-openapi.yml
- filename: quicknode-streams-api-openapi.yml
  format: yaml
  label: QuickNode Streams API
  slug: quicknode-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-streams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Quicknode Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuickNode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QuickNode
provider_slug: quicknode
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/quicknode-ipfs-openapi.yml
  - openapi/quicknode-key-value-store-openapi.yml
  - openapi/quicknode-streams-openapi.yml
  type: apiKey
slug: quicknode-authentication
source_filename: quicknode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quicknode-ipfs-openapi.yml, openapi/quicknode-key-value-store-openapi.yml, openapi/quicknode-streams-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/quicknode-ipfs-openapi.yml\n  - openapi/quicknode-key-value-store-openapi.yml\n  - openapi/quicknode-streams-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/authentication/quicknode-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Blockchain
- RPC
- Streams
- IPFS
- Multi-chain
---
