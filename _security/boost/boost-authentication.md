---
api_key_in: []
api_specs:
- filename: boost-v2-openapi.json
  format: json
  label: Boost V2 API
  slug: boost-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-v2-openapi.json
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Boost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boost secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boost
provider_slug: boost
scheme_count: 1
schemes:
- detail: 'The Boost V2 read API (https://api-v2.boost.xyz) is public and requires no authentication — no API key, bearer token, or OAuth. The docs'' API examples issue unauthenticated requests directly against the endpoint. State changes occur on-chain (wallet-signed transactions) via the protocol contracts and SDK, not through authenticated REST calls.

    '
  name: public
  sources:
  - openapi/boost-v2-openapi.json
  type: none
slug: boost-authentication
source_filename: boost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.boost.xyz/v2/boost-api/fetch-boosts\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: public\n    type: none\n    detail: >\n      The Boost V2 read API (https://api-v2.boost.xyz) is public and requires no\n      authentication — no API key, bearer token, or OAuth. The docs' API examples\n      issue unauthenticated requests directly against the endpoint. State changes\n      occur on-chain (wallet-signed transactions) via the protocol contracts and\n      SDK, not through authenticated REST calls.\n    sources: [openapi/boost-v2-openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/authentication/boost-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Crypto
- Web3
- Incentives
- Rewards
- Blockchain
- DeFi
- Onchain
- EVM
---
