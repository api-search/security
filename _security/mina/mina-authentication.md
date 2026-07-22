---
api_key_in: []
auth_types:
- none
- passphrase-unlock
description: ''
kind: authentication
layout: security
method: searched
name: Mina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mina secures its APIs with none and passphrase-unlock across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mina
provider_slug: mina
scheme_count: 3
schemes:
- detail: GraphQL endpoint bound to localhost; exposing it to the internet lets anyone spend from known accounts.
  name: network-boundary
  sources:
  - graphql/mina-graphql-schema.json
  type: none
- detail: Accounts are unlocked with a passphrase before signing; MINA_PRIVKEY_PASS supplies it in daemon/sandbox startup.
  name: account-passphrase
  operations:
  - unlockAccount
  - lockAccount
  - unlockWallet
  - lockWallet
  sources:
  - graphql/mina-graphql-schema.json
  type: passphrase
- detail: Payments/delegations/zkApp commands are signed with the account private key (mina-signer / o1js).
  name: transaction-signature
  sources:
  - https://www.npmjs.com/package/mina-signer
  type: cryptographic-signature
slug: mina-authentication
source_filename: mina-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.minaprotocol.com/node-developers/graphql-api\nsummary:\n  types: [none, passphrase-unlock]\n  api_key_in: []\n  oauth2_flows: []\n  model: network-boundary + per-account passphrase\ndetail: >-\n  The Mina daemon GraphQL API has no token, API-key, or OAuth authentication.\n  Security is enforced by network boundary: the GraphQL port (3085) binds to\n  localhost by default and only accepts localhost connections unless the operator\n  passes -insecure-rest-server. Individual accounts are protected by a passphrase\n  and must be unlocked (unlockAccount) before they can sign/send transactions,\n  then re-locked (lockAccount). Transaction authorization is cryptographic: each\n  command is signed with the account's private key (see the mina-signer library).\nschemes:\n  - name: network-boundary\n    type: none\n    detail: GraphQL endpoint bound to localhost; exposing it to the internet lets anyone spend from known accounts.\n\
  \    sources: [graphql/mina-graphql-schema.json]\n  - name: account-passphrase\n    type: passphrase\n    operations: [unlockAccount, lockAccount, unlockWallet, lockWallet]\n    detail: Accounts are unlocked with a passphrase before signing; MINA_PRIVKEY_PASS supplies it in daemon/sandbox startup.\n    sources: [graphql/mina-graphql-schema.json]\n  - name: transaction-signature\n    type: cryptographic-signature\n    detail: Payments/delegations/zkApp commands are signed with the account private key (mina-signer / o1js).\n    sources: [https://www.npmjs.com/package/mina-signer]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mina/refs/heads/main/authentication/mina-authentication.yml
summary_line: none/passphrase-unlock · 3 schemes
tags:
- Company
- Crypto
- Blockchain
- Zero-Knowledge
- zkApps
- GraphQL
- Web3
- Cryptocurrency
---
