---
api_key_in:
- sdk-config
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rly Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: RLY Network secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RLY Network
provider_slug: rly-network
scheme_count: 1
schemes:
- description: A project API key obtained from the RallyProtocol dashboard is passed into the SDK at initialization (e.g. RlyNetwork.configureMumbai / getAccount flows). The key scopes gasless-transaction relaying and dashboard usage; wallet keys themselves are generated and held on-device in the secure enclave, never sent to Rally.
  name: RallyApiKey
  obtain_at: https://app.rallyprotocol.com/
  sources:
  - docs.rallyprotocol.com
  type: apiKey
slug: rly-network-authentication
source_filename: rly-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.rallyprotocol.com/\ndocs: https://docs.rallyprotocol.com/react-native-expo/getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [sdk-config]\n  oauth2_flows: []\nschemes:\n  - name: RallyApiKey\n    type: apiKey\n    description: >-\n      A project API key obtained from the RallyProtocol dashboard is passed into\n      the SDK at initialization (e.g. RlyNetwork.configureMumbai / getAccount\n      flows). The key scopes gasless-transaction relaying and dashboard usage;\n      wallet keys themselves are generated and held on-device in the secure\n      enclave, never sent to Rally.\n    obtain_at: https://app.rallyprotocol.com/\n    sources: [docs.rallyprotocol.com]\nnotes: >-\n  RLY Network publishes no OpenAPI/REST surface; authentication is an SDK\n  configuration concern (project API key + on-device key custody) rather than a\n  server securityScheme. Captured from the developer docs, not derived from\
  \ a\n  spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rly-network/refs/heads/main/authentication/rly-network-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Web3
- Blockchain
- Wallets
- Mobile SDK
- Gasless Transactions
- Cryptocurrency
- Developer Tools
---
