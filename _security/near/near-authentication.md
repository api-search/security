---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: NEAR RPC API
  slug: near-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/openapi.yml
- filename: fastnear-api.json
  format: json
  label: FASTNEAR Indexed REST API
  slug: fastnear-indexed-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/openapi/fastnear-api.json
- filename: nearblocks-api.json
  format: json
  label: NearBlocks Explorer API
  slug: nearblocks-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/openapi/nearblocks-api.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Near Authentication
name_suffix: Authentication
oauth_flows: []
overview: NEAR Protocol secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NEAR Protocol
provider_slug: near
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nearblocks-api.json
  type: http
slug: near-authentication
source_filename: near-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nearblocks-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nearblocks-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/authentication/near-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Web3
- NEAR
- NFT
- Tokens
- Staking
- Crypto
---
