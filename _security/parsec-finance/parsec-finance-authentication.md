---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Parsec Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parsec Finance secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parsec Finance
provider_slug: parsec-finance
scheme_count: 1
schemes:
- in: header
  key_prefix: par_ak_
  name: ApiKey
  notes: All requests are POSTed to the single GraphQL endpoint https://api.parsec.finance/api/v2 with the API key supplied in an `api_key` request header. API access requires a Pro subscription. There is no OAuth or scope surface — a single account-level key authorizes the full GraphQL query surface.
  parameter_name: api_key
  provisioning: Parsec app -> Settings -> Subscription -> api key
  sources:
  - graphql/parsec-finance-api.graphql
  type: apiKey
slug: parsec-finance-authentication
source_filename: parsec-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/parsec-finance/parsec_python_sdk (parsecfi/parsecfi.py) + https://docs.parsec.finance/\ndocs: https://docs.parsec.finance/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter_name: api_key\n  key_prefix: par_ak_\n  provisioning: Parsec app -> Settings -> Subscription -> api key\n  notes: >-\n    All requests are POSTed to the single GraphQL endpoint\n    https://api.parsec.finance/api/v2 with the API key supplied in an `api_key`\n    request header. API access requires a Pro subscription. There is no OAuth or\n    scope surface — a single account-level key authorizes the full GraphQL query\n    surface.\n  sources: [graphql/parsec-finance-api.graphql]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsec-finance/refs/heads/main/authentication/parsec-finance-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Analytics
- DeFi
- NFT
- Blockchain
- Cryptocurrency
- On-Chain Data
- Web3
- GraphQL
- Trading
---
