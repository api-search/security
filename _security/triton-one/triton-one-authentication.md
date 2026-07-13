---
api_key_in:
- header
api_specs:
- filename: triton-one-customers-api-openapi.yml
  format: yaml
  label: Triton One Customers API
  slug: triton-one-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triton-one/refs/heads/main/openapi/triton-one-customers-api-openapi.yml
- filename: triton-one-solana-rpc-api-openapi.yml
  format: yaml
  label: Triton One Solana RPC API
  slug: triton-one-solana-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triton-one/refs/heads/main/openapi/triton-one-solana-rpc-api-openapi.yml
- filename: triton-one-digital-assets-api-openapi.yml
  format: yaml
  label: Triton One Digital Assets API
  slug: triton-one-digital-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triton-one/refs/heads/main/openapi/triton-one-digital-assets-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Triton One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Triton One secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Triton One
provider_slug: triton-one
scheme_count: 2
schemes:
- description: Customers API token passed in Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/triton-one-customers-api-openapi.yml
  type: http
- description: RPC consumption token from Customers API.
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/triton-one-digital-assets-api-openapi.yml
  - openapi/triton-one-solana-rpc-api-openapi.yml
  type: apiKey
slug: triton-one-authentication
source_filename: triton-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/triton-one-customers-api-openapi.yml, openapi/triton-one-digital-assets-api-openapi.yml,\n  openapi/triton-one-solana-rpc-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Customers API token passed in Authorization header.\n  sources:\n  - openapi/triton-one-customers-api-openapi.yml\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: RPC consumption token from Customers API.\n  sources:\n  - openapi/triton-one-digital-assets-api-openapi.yml\n  - openapi/triton-one-solana-rpc-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triton-one/refs/heads/main/authentication/triton-one-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Solana
- RPC
- Blockchain
- Web3
- Streaming
- Yellowstone
- Validator
- gRPC
- Pythnet
- Sui
- Monad
---
