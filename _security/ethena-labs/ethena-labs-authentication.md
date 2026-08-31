---
api_key_in: []
auth_types:
- ip-allowlist
- wallet-allowlist
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Ethena Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ethena Labs secures its APIs with ip-allowlist, wallet-allowlist, and signature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ethena Labs
provider_slug: ethena-labs
scheme_count: 4
schemes:
- description: Callers must have their IP address whitelisted by Ethena. The private endpoint (https://private.api.ethena.fi) requires IP whitelisting; the public endpoint (https://public.api.ethena.fi) is reachable but only whitelisted wallets can transact.
  name: ip-allowlist
  type: network
- description: The benefactor (and, where different, beneficiary) Ethereum wallet address must be whitelisted onchain by Ethena. Non-whitelisted addresses are rejected (error codes 10, 25, 26).
  name: wallet-allowlist
  type: onchain-identity
- description: Default order authentication. The caller signs the typed order object (order_id, order type, expiry, nonce, benefactor/beneficiary, collateral asset + amount, USDe amount) and submits the hex signature on the POST /order request. Nonces prevent replay (error 24 on duplicate nonce).
  name: eip712-signature
  scheme: EIP-712
  type: signature
- description: Alternative signature type for smart-contract wallets. Supplied by appending signature_type=EIP1271 to the POST /order request.
  name: eip1271-signature
  scheme: EIP-1271
  type: signature
slug: ethena-labs-authentication
source_filename: ethena-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.ethena.fi/api-documentation/overview\ndocs: https://docs.ethena.fi/api-documentation/overview\nsummary:\n  types: [ip-allowlist, wallet-allowlist, signature]\n  notes: >-\n    The Ethena Minting API does not use API keys or bearer tokens. Access is gated at two layers:\n    network-level IP whitelisting and onchain wallet-address whitelisting (benefactor / beneficiary).\n    Order submission is authenticated by a cryptographic signature over the EIP-712 typed order\n    payload, so authority derives from control of the whitelisted wallet's private key rather than a\n    shared secret.\nschemes:\n- name: ip-allowlist\n  type: network\n  description: >-\n    Callers must have their IP address whitelisted by Ethena. The private endpoint\n    (https://private.api.ethena.fi) requires IP whitelisting; the public endpoint\n    (https://public.api.ethena.fi) is reachable but only whitelisted wallets can transact.\n- name:\
  \ wallet-allowlist\n  type: onchain-identity\n  description: >-\n    The benefactor (and, where different, beneficiary) Ethereum wallet address must be whitelisted\n    onchain by Ethena. Non-whitelisted addresses are rejected (error codes 10, 25, 26).\n- name: eip712-signature\n  type: signature\n  scheme: EIP-712\n  description: >-\n    Default order authentication. The caller signs the typed order object (order_id, order type,\n    expiry, nonce, benefactor/beneficiary, collateral asset + amount, USDe amount) and submits the\n    hex signature on the POST /order request. Nonces prevent replay (error 24 on duplicate nonce).\n- name: eip1271-signature\n  type: signature\n  scheme: EIP-1271\n  description: >-\n    Alternative signature type for smart-contract wallets. Supplied by appending\n    signature_type=EIP1271 to the POST /order request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethena-labs/refs/heads/main/authentication/ethena-labs-authentication.yml
summary_line: ip-allowlist/wallet-allowlist/signature · 4 schemes
tags:
- Company
- Crypto
- Stablecoin
- DeFi
- Synthetic Dollar
- Minting
- Blockchain
- Ethereum
---
