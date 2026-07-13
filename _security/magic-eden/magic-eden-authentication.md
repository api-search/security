---
api_key_in: []
api_specs:
- filename: magic-eden-solana-openapi.yml
  format: yaml
  label: Magic Eden Solana API
  slug: solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/openapi/magic-eden-solana-openapi.yml
- filename: magic-eden-evm-openapi.yml
  format: yaml
  label: Magic Eden EVM API
  slug: evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/openapi/magic-eden-evm-openapi.yml
- filename: magic-eden-ordinals-openapi.yml
  format: yaml
  label: Magic Eden Bitcoin Ordinals & Runes API
  slug: ordinals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/openapi/magic-eden-ordinals-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Magic Eden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magic Eden secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Magic Eden
provider_slug: magic-eden
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/magic-eden-evm-openapi.yml
  - openapi/magic-eden-ordinals-openapi.yml
  - openapi/magic-eden-solana-openapi.yml
  type: http
slug: magic-eden-authentication
source_filename: magic-eden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/magic-eden-evm-openapi.yml, openapi/magic-eden-ordinals-openapi.yml, openapi/magic-eden-solana-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/magic-eden-evm-openapi.yml\n  - openapi/magic-eden-ordinals-openapi.yml\n  - openapi/magic-eden-solana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/authentication/magic-eden-authentication.yml
summary_line: http · 1 scheme
tags:
- NFT
- Web3
- Blockchain
- Marketplace
- Solana
- Ethereum
- Bitcoin
- Ordinals
- Runes
- Multi-chain
---
