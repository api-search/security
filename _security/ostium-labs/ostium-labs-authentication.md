---
api_key_in: []
api_specs:
- filename: ostium-labs-prices-asyncapi.yml
  format: yaml
  label: Ostium Builder API
  slug: ostium-builder-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostium-labs/refs/heads/main/asyncapi/ostium-labs-prices-asyncapi.yml
auth_types:
- wallet-signature
- delegated-key
- public-read
description: ''
kind: authentication
layout: security
method: searched
name: Ostium Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ostium Labs secures its APIs with wallet-signature, delegated-key, and public-read across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ostium Labs
provider_slug: ostium-labs
scheme_count: 3
schemes:
- description: Trader-owned positions signed directly by the trader's EOA (self + self / self + gasless modes). The connected trader address authorizes on-chain actions via wallet signatures; Safe-based gasless modes submit sponsored user operations.
  modes:
  - self-and-self
  - self-and-gasless
  name: trader-wallet-signature
  type: wallet-signature
- description: Backend-controlled delegated execution. A delegate address/EOA registered via setDelegate signs and (optionally) pays gas on behalf of a trader. The delegate private key is generated/exported from the Ostium app.
  modes:
  - delegated-and-self
  - delegated-and-gasless
  name: delegate-key
  setup_operations:
  - setDelegate
  - removeDelegate
  - setupGaslessDelegation
  type: delegated-key
- description: Read-only market and account data (createReadOnly mode) and the public Builder API endpoints require no authentication.
  modes:
  - read-only
  name: public-read
  type: none
slug: ostium-labs-authentication
source_filename: ostium-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.ostium.com/developer/client-modes/overview\nsummary:\n  types: [wallet-signature, delegated-key, public-read]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Ostium is a self-custodial DeFi protocol; there is no server-side API key or\n    OAuth. Authentication and authorization happen at the wallet / smart-contract\n    layer. The public Builder API read endpoints (prices, OHLC, subgraph, price\n    stream) require no credentials.\nschemes:\n- name: trader-wallet-signature\n  type: wallet-signature\n  description: >-\n    Trader-owned positions signed directly by the trader's EOA (self + self / self +\n    gasless modes). The connected trader address authorizes on-chain actions via\n    wallet signatures; Safe-based gasless modes submit sponsored user operations.\n  modes: [self-and-self, self-and-gasless]\n- name: delegate-key\n  type: delegated-key\n  description: >-\n    Backend-controlled delegated\
  \ execution. A delegate address/EOA registered via\n    setDelegate signs and (optionally) pays gas on behalf of a trader. The delegate\n    private key is generated/exported from the Ostium app.\n  modes: [delegated-and-self, delegated-and-gasless]\n  setup_operations: [setDelegate, removeDelegate, setupGaslessDelegation]\n- name: public-read\n  type: none\n  description: >-\n    Read-only market and account data (createReadOnly mode) and the public Builder\n    API endpoints require no authentication.\n  modes: [read-only]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ostium-labs/refs/heads/main/authentication/ostium-labs-authentication.yml
summary_line: wallet-signature/delegated-key/public-read · 3 schemes
tags:
- Company
- Perpetual Futures
- Decentralized Finance
- DeFi
- Trading
- Real World Assets
- Derivatives
- Arbitrum
- Blockchain
- Web3
- Market Data
- SDK
---
