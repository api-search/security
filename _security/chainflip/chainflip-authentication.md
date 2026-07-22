---
api_key_in: []
auth_types:
- none
- node-operated
description: Chainflip is a permissionless, non-custodial protocol. Its integration surfaces do not use API keys, bearer tokens, or OAuth. Access is either fully open (public RPC / quoting) or gated by operating a node account whose authority derives from on-chain identity and cryptographic signatures.
kind: authentication
layout: security
method: searched
name: Chainflip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chainflip secures its APIs with none and node-operated across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chainflip
provider_slug: chainflip
scheme_count: 4
schemes:
- applies_to: SDK quoting and swap initiation (getChains, getAssets, getQuoteV2, requestDepositAddressV2, getStatusV2)
  name: public-rpc
  notes: No credentials required. Calls hit the public Chainflip RPC node for the selected network, or a custom rpcUrl.
  type: none
- applies_to: Broker API (routing swaps, earning broker commission)
  name: broker-account
  notes: Authority comes from running/connecting to a Broker node registered on the State Chain; broker actions are authorised by the broker account's keypair, not an HTTP API key. A hosted Broker API URL may be supplied via the SDK `broker` option.
  type: node-operated
- applies_to: Liquidity Provider RPC / LP operations
  name: lp-account
  notes: LP actions are signed by the LP account keypair on the State Chain.
  type: node-operated
- applies_to: Validator node operation and governance
  name: validator-keys
  notes: Validator/governance transactions are signed with node keys (see cf-gov and cf-trezor-signer CLI tools).
  type: node-operated
slug: chainflip-authentication
source_filename: chainflip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chainflip.io/brokers/how-to-use-chainflip-sdk\nsummary:\n  types: [none, node-operated]\n  api_key_in: []\n  oauth2_flows: []\ndescription: >-\n  Chainflip is a permissionless, non-custodial protocol. Its integration\n  surfaces do not use API keys, bearer tokens, or OAuth. Access is either\n  fully open (public RPC / quoting) or gated by operating a node account whose\n  authority derives from on-chain identity and cryptographic signatures.\nschemes:\n  - name: public-rpc\n    type: none\n    applies_to: SDK quoting and swap initiation (getChains, getAssets, getQuoteV2, requestDepositAddressV2, getStatusV2)\n    notes: No credentials required. Calls hit the public Chainflip RPC node for the selected network, or a custom rpcUrl.\n  - name: broker-account\n    type: node-operated\n    applies_to: Broker API (routing swaps, earning broker commission)\n    notes: >-\n      Authority comes from running/connecting to\
  \ a Broker node registered on\n      the State Chain; broker actions are authorised by the broker account's\n      keypair, not an HTTP API key. A hosted Broker API URL may be supplied via\n      the SDK `broker` option.\n  - name: lp-account\n    type: node-operated\n    applies_to: Liquidity Provider RPC / LP operations\n    notes: LP actions are signed by the LP account keypair on the State Chain.\n  - name: validator-keys\n    type: node-operated\n    applies_to: Validator node operation and governance\n    notes: Validator/governance transactions are signed with node keys (see cf-gov and cf-trezor-signer CLI tools).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainflip/refs/heads/main/authentication/chainflip-authentication.yml
summary_line: none/node-operated · 4 schemes
tags:
- Company
- Crypto
- Blockchain
- DeFi
- Cross-Chain
- Swaps
- Bridge
- Lending
- Liquidity
- Web3
---
