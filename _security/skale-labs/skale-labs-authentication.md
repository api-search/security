---
api_key_in: []
auth_types:
- none
- wallet-signature
description: 'SKALE surfaces are Ethereum-compatible JSON-RPC endpoints and SDKs, not key-authenticated REST APIs. Public JSON-RPC RPC endpoints (skalenodes.com) require no API key. State-changing operations are authenticated cryptographically: transactions are signed with an EVM wallet private key (ECDSA/secp256k1) and gas is paid via sFUEL / CREDITs rather than an account token.'
kind: authentication
layout: security
method: searched
name: Skale Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skale Labs secures its APIs with none and wallet-signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Skale Labs
provider_slug: skale-labs
scheme_count: 3
schemes:
- description: Read methods (eth_call, eth_getBalance, eth_blockNumber, ...) over public HTTPS/WSS JSON-RPC endpoints; no credential required.
  name: public-json-rpc
  sources:
  - https://docs.skale.space/developers/resources/json-rpc-api
  type: none
- description: Write operations (eth_sendRawTransaction) require a transaction signed by the sender's EVM private key. SDKs (BITE, MPP) and the SKALE CLI manage signing.
  name: wallet-signature
  scheme: eip155-signature
  sources:
  - https://docs.skale.space/developers/sdks/skalenetwork-cli
  type: wallet
- description: Watchdog node-status REST API (port 3009) exposes public read-only status endpoints; no auth documented.
  name: watchdog-rest
  sources:
  - https://docs.skale.space/validators/watchdog/apis
  type: none
slug: skale-labs-authentication
source_filename: skale-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.skale.space/developers/resources/json-rpc-api\nsummary:\n  types: [none, wallet-signature]\n  api_key_in: []\n  oauth2_flows: []\ndescription: >-\n  SKALE surfaces are Ethereum-compatible JSON-RPC endpoints and SDKs, not key-authenticated REST\n  APIs. Public JSON-RPC RPC endpoints (skalenodes.com) require no API key. State-changing operations\n  are authenticated cryptographically: transactions are signed with an EVM wallet private key\n  (ECDSA/secp256k1) and gas is paid via sFUEL / CREDITs rather than an account token.\nschemes:\n  - name: public-json-rpc\n    type: none\n    description: Read methods (eth_call, eth_getBalance, eth_blockNumber, ...) over public HTTPS/WSS JSON-RPC endpoints; no credential required.\n    sources: [https://docs.skale.space/developers/resources/json-rpc-api]\n  - name: wallet-signature\n    type: wallet\n    scheme: eip155-signature\n    description: Write operations (eth_sendRawTransaction)\
  \ require a transaction signed by the sender's EVM private key. SDKs (BITE, MPP) and the SKALE CLI manage signing.\n    sources: [https://docs.skale.space/developers/sdks/skalenetwork-cli]\n  - name: watchdog-rest\n    type: none\n    description: Watchdog node-status REST API (port 3009) exposes public read-only status endpoints; no auth documented.\n    sources: [https://docs.skale.space/validators/watchdog/apis]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skale-labs/refs/heads/main/authentication/skale-labs-authentication.yml
summary_line: none/wallet-signature · 3 schemes
tags:
- Company
- Blockchain
- Web3
- Smart Contracts
- Developer Tools
- JSON-RPC
- AI Agents
- Privacy
- Payments
- Cryptocurrency
---
