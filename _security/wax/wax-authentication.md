---
api_key_in: []
auth_types:
- none
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Wax Authentication
name_suffix: Authentication
oauth_flows: []
overview: WAX secures its APIs with none and signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WAX
provider_slug: wax
scheme_count: 3
schemes:
- applies_to: Chain API (/v1/chain/*) and Hyperion History API (/v1/history/*, /v2/*) read endpoints
  description: Read RPC endpoints are public and require no credential. Requests are HTTP POST (or GET for some Hyperion routes) with a JSON body.
  name: public-read
  type: none
- applies_to: /v1/chain/push_transaction, /v1/chain/send_transaction
  description: State-changing actions must be packed and signed client-side with the account's active/owner key. Signatures are secp256k1 (EOSIO/Antelope "K1"). The WAX Cloud Wallet (all-access.wax.io) brokers signing for users via wax.login()/wax.api.transact() in @waxio/waxjs; self-custody wallets sign locally. The chain verifies the signature against the account's permission/authority, not against a server-issued token.
  name: transaction-signature
  scheme: antelope-eosio (secp256k1 / ecc)
  type: signature
- applies_to: WAX Cloud Wallet login flow
  description: End users authenticate to the WAX Cloud Wallet via email or social SSO at all-access.wax.io; the wallet then signs on their behalf. This is an end-user auth flow, not an API credential a developer provisions.
  name: wax-cloud-wallet-sso
  type: session
slug: wax-authentication
source_filename: wax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.wax.io/ , https://github.com/worldwide-asset-exchange/waxjs\nnotes: >-\n  WAX is an Antelope (EOSIO fork) blockchain. There is no OpenAPI in the repo to\n  derive from; this profile is authored from the public docs and the official\n  waxjs SDK. The public Chain/History (Hyperion) RPC read endpoints are\n  unauthenticated; state-changing calls are authorized by client-side\n  cryptographic signatures over the transaction, produced by a user key or via\n  the WAX Cloud Wallet — not by API keys, OAuth, or bearer tokens.\nsummary:\n  types: [none, signature]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: public-read\n    type: none\n    applies_to: Chain API (/v1/chain/*) and Hyperion History API (/v1/history/*, /v2/*) read endpoints\n    description: >-\n      Read RPC endpoints are public and require no credential. Requests are\n      HTTP POST (or GET for some Hyperion routes) with a JSON body.\n  -\
  \ name: transaction-signature\n    type: signature\n    scheme: antelope-eosio (secp256k1 / ecc)\n    applies_to: /v1/chain/push_transaction, /v1/chain/send_transaction\n    description: >-\n      State-changing actions must be packed and signed client-side with the\n      account's active/owner key. Signatures are secp256k1 (EOSIO/Antelope\n      \"K1\"). The WAX Cloud Wallet (all-access.wax.io) brokers signing for users\n      via wax.login()/wax.api.transact() in @waxio/waxjs; self-custody wallets\n      sign locally. The chain verifies the signature against the account's\n      permission/authority, not against a server-issued token.\n  - name: wax-cloud-wallet-sso\n    type: session\n    applies_to: WAX Cloud Wallet login flow\n    description: >-\n      End users authenticate to the WAX Cloud Wallet via email or social SSO at\n      all-access.wax.io; the wallet then signs on their behalf. This is an\n      end-user auth flow, not an API credential a developer provisions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wax/refs/heads/main/authentication/wax-authentication.yml
summary_line: none/signature · 3 schemes
tags:
- Company
- Crypto
- Blockchain
- NFT
- Web3
- Gaming
- Antelope
- Wallet
---
