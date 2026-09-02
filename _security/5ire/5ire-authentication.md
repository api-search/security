---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: 5Ire Authentication
name_suffix: Authentication
oauth_flows: []
overview: 5ire secures its APIs with none across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 5ire
provider_slug: 5ire
scheme_count: 3
schemes:
- description: Public, unauthenticated Ethereum JSON-RPC 2.0. No credential is accepted or required.
  name: none
  sources:
  - https://docs.5ire.org/build-on-5irechain/evm-compatibility/
  surface: 5ireChain Mainnet JSON-RPC (https://rpc.5ire.network)
  type: none
- description: Public, unauthenticated Ethereum JSON-RPC 2.0.
  name: none
  sources:
  - https://docs.5ire.org/wallets/metamask/
  surface: 5ireChain Thunder Testnet JSON-RPC (https://rpc.testnet.5ire.network)
  type: none
- description: Public Substrate RPC. Self-hosted nodes gate exposure with node CLI flags (--rpc-external, --rpc-cors, --rpc-methods) rather than with credentials.
  name: none
  sources:
  - https://github.com/5ire-tech/5ireChain
  surface: 5ireChain Native Substrate RPC (WebSocket, port 9944)
  type: none
slug: 5ire-authentication
source_filename: 5ire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: >-\n  https://docs.5ire.org/build-on-5irechain/evm-compatibility/, https://docs.5ire.org/wallets/metamask/,\n  https://github.com/5ire-tech/5ireChain (README node flags), ethereum-lists/chains entries 995 and 997.\n  Content verified via Internet Archive captures (2025-02 / 2025-03); live origin returned HTTP 530 on 2026-08-02.\ndocs: https://docs.5ire.org/build-on-5irechain/evm-compatibility/\nsummary:\n  types:\n    - none\n  api_key_in: []\n  oauth2_flows: []\n  transport_auth: false\n  request_auth: cryptographic-signature\n  note: >-\n    5ireChain exposes no HTTP-layer authentication. The public JSON-RPC endpoints accept anonymous requests with no\n    API key, bearer token, basic credential, OAuth 2.0 flow, OpenID Connect issuer or mutual TLS. Authorization is\n    not an API concern at all: read methods are unauthenticated by design, and any state-changing call is an\n    ECDSA-signed transaction (secp256k1 on the EVM\
  \ side, sr25519/ed25519 on the native Substrate side) whose\n    authority comes from the signing key held in the caller's wallet, not from a credential presented to the\n    endpoint. There are consequently no scopes, no token lifetimes and no scopes/ artifact for this provider.\nschemes:\n  - name: none\n    type: none\n    surface: 5ireChain Mainnet JSON-RPC (https://rpc.5ire.network)\n    description: Public, unauthenticated Ethereum JSON-RPC 2.0. No credential is accepted or required.\n    sources:\n      - https://docs.5ire.org/build-on-5irechain/evm-compatibility/\n  - name: none\n    type: none\n    surface: 5ireChain Thunder Testnet JSON-RPC (https://rpc.testnet.5ire.network)\n    description: Public, unauthenticated Ethereum JSON-RPC 2.0.\n    sources:\n      - https://docs.5ire.org/wallets/metamask/\n  - name: none\n    type: none\n    surface: 5ireChain Native Substrate RPC (WebSocket, port 9944)\n    description: >-\n      Public Substrate RPC. Self-hosted nodes gate exposure\
  \ with node CLI flags (--rpc-external, --rpc-cors,\n      --rpc-methods) rather than with credentials.\n    sources:\n      - https://github.com/5ire-tech/5ireChain\ntransaction_signing:\n  evm:\n    curve: secp256k1\n    scheme: ECDSA\n    chain_id_binding: EIP-155 (995 mainnet / 997 Thunder testnet)\n    replay_protection: per-account nonce plus chain-ID binding\n    wallets:\n      - MetaMask\n      - 5ire Wallet browser extension\n    docs: https://docs.5ire.org/wallets/metamask/\n  native:\n    curves:\n      - sr25519\n      - ed25519\n    scheme: Substrate SignedExtrinsic\n    replay_protection: per-account nonce plus mortal era and genesis-hash binding\n    wallets:\n      - 5ire Wallet browser extension\n    docs: https://docs.5ire.org/wallets/5ire-wallet-extension/\ngaps:\n  - No API-key or token issuance surface exists, so there is no key rotation, revocation or scope model to document.\n  - No OpenAPI document is published, so no securitySchemes could be derived mechanically.\n\
  \  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server was retrievable on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/5ire/refs/heads/main/authentication/5ire-authentication.yml
summary_line: none · 3 schemes
tags:
- Blockchain
- Layer 1
- Smart Contracts
- EVM
- Web3
- Substrate
- JSON-RPC
- Sustainability
- ESG
- Proof of Stake
- Cryptocurrency
- Developer Tools
---
