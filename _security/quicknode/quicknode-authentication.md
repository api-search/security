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
- filename: quicknode-streams-openapi.yml
  format: yaml
  label: QuickNode Streams
  slug: streams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-streams-openapi.yml
- filename: quicknode-ipfs-openapi.yml
  format: yaml
  label: QuickNode IPFS API
  slug: ipfs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-ipfs-openapi.yml
- filename: quicknode-key-value-store-openapi.yml
  format: yaml
  label: QuickNode Key-Value Store
  slug: kv-store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-key-value-store-openapi.yml
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
