---
api_key_in: []
api_specs:
- filename: boost-action-api-openapi.yml
  format: yaml
  label: Boost Action API
  slug: boost-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-action-api-openapi.yml
- filename: boost-action-template-api-openapi.yml
  format: yaml
  label: Boost Action Template API
  slug: boost-action-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-action-template-api-openapi.yml
- filename: boost-blocklist-api-openapi.yml
  format: yaml
  label: Boost Blocklist API
  slug: boost-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-blocklist-api-openapi.yml
- filename: boost-boost-api-openapi.yml
  format: yaml
  label: Boost Boost API
  slug: boost-boost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-boost-api-openapi.yml
- filename: boost-budget-api-openapi.yml
  format: yaml
  label: Boost Budget API
  slug: boost-budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-budget-api-openapi.yml
- filename: boost-contract-api-openapi.yml
  format: yaml
  label: Boost Contract API
  slug: boost-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-contract-api-openapi.yml
- filename: boost-rewardkit-api-openapi.yml
  format: yaml
  label: Boost RewardKit API
  slug: boost-rewardkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-rewardkit-api-openapi.yml
- filename: boost-rewardkittrending-api-openapi.yml
  format: yaml
  label: Boost RewardKitTrending API
  slug: boost-rewardkittrending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-rewardkittrending-api-openapi.yml
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
