---
api_key_in: []
auth_types:
- wallet-connect
description: ''
kind: authentication
layout: security
method: searched
name: Sender Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sender secures its APIs with wallet-connect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sender
provider_slug: sender
scheme_count: 2
schemes:
- chain: near
  docs: https://docs.senderwallet.io/guide/sign-in-applications/sign-in-applications-in-near
  methods:
  - requestSignIn
  - signOut
  - isSignedIn
  - getAccountId
  name: near-sign-in
  type: wallet-connect
- chain: ethereum
  docs: https://docs.senderwallet.io/guide/sign-in-applications/sign-in-applications-in-ethereum
  methods:
  - eth_requestAccounts
  - wallet_requestPermissions
  - wallet_getPermissions
  name: ethereum-account-access
  standard: EIP-1102
  type: wallet-connect
slug: sender-authentication
source_filename: sender-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.senderwallet.io/guide/sign-in-applications\ndocs: https://docs.senderwallet.io/guide/sign-in-applications\nsummary:\n  types: [wallet-connect]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Sender is a self-custody Web3 wallet. Authentication is user approval of a\n    connection/sign-in request inside the wallet UI, not a server credential.\nschemes:\n  - name: near-sign-in\n    type: wallet-connect\n    chain: near\n    methods:\n      - requestSignIn   # request an access key scoped to a contract account\n      - signOut         # clear the signed-in access key\n      - isSignedIn      # check for an active session\n      - getAccountId    # read the selected NEAR account id\n    docs: https://docs.senderwallet.io/guide/sign-in-applications/sign-in-applications-in-near\n  - name: ethereum-account-access\n    type: wallet-connect\n    chain: ethereum\n    standard: EIP-1102\n    methods:\n      - eth_requestAccounts\
  \    # prompt the user to expose an address\n      - wallet_requestPermissions\n      - wallet_getPermissions\n    docs: https://docs.senderwallet.io/guide/sign-in-applications/sign-in-applications-in-ethereum\nsigning:\n  near: [signAndSendTransaction, requestSignTransactions]\n  ethereum: [eth_sendTransaction, personal_sign]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sender/refs/heads/main/authentication/sender-authentication.yml
summary_line: wallet-connect · 2 schemes
tags:
- Company
- Crypto
- Wallet
- Web3
- Blockchain
- Ethereum
- NEAR
- DeFi
- Self-Custody
---
