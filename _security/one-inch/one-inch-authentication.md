---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: One Inch Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1inch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 1inch
provider_slug: one-inch
scheme_count: 1
schemes:
- description: 'API key issued from https://portal.1inch.dev passed as

    `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/one-inch-openapi.yml
  type: http
slug: one-inch-authentication
source_filename: one-inch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/one-inch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API key issued from https://portal.1inch.dev passed as\n    `Authorization: Bearer <token>`.\n  sources:\n  - openapi/one-inch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-inch/refs/heads/main/authentication/one-inch-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- DeFi
- DEX
- Aggregator
- Swap
- Multi-chain
- Limit Orders
- Fusion
- Cross-chain
---
