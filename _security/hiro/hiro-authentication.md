---
api_key_in:
- header
api_specs:
- filename: hiro-stacks-blockchain-api-openapi.yaml
  format: yaml
  label: Stacks Blockchain API
  slug: stacks-blockchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-stacks-blockchain-api-openapi.yaml
- filename: hiro-stacks-node-rpc-api-openapi.yaml
  format: yaml
  label: Stacks Node RPC API
  slug: stacks-node-rpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-stacks-node-rpc-api-openapi.yaml
- filename: hiro-token-metadata-api-openapi.yaml
  format: yaml
  label: Hiro Token Metadata API
  slug: token-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-token-metadata-api-openapi.yaml
- filename: hiro-signer-metrics-api-openapi.yaml
  format: yaml
  label: Hiro Signer Metrics API
  slug: signer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-signer-metrics-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hiro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hiro secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hiro
provider_slug: hiro
scheme_count: 1
schemes:
- description: 'Plain-text secret value that must exactly equal the node''s

    configured password, which is set as `connection_options.auth_token`

    in the node''s configuration file.'
  in: header
  name: rpcAuth
  parameter: authorization
  sources:
  - openapi/hiro-stacks-node-rpc-api-openapi.yaml
  type: apiKey
slug: hiro-authentication
source_filename: hiro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hiro-stacks-node-rpc-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: rpcAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: |-\n    Plain-text secret value that must exactly equal the node's\n    configured password, which is set as `connection_options.auth_token`\n    in the node's configuration file.\n  sources:\n  - openapi/hiro-stacks-node-rpc-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/authentication/hiro-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Blockchain
- Bitcoin
- Stacks
- sBTC
- Indexing
---
