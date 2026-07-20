---
api_key_in: []
auth_types:
- derived-keys
- message-signing
description: ''
kind: authentication
layout: security
method: searched
name: Bitclout Deso Authentication
name_suffix: Authentication
oauth_flows: []
overview: BitClout (DeSo) secures its APIs with derived-keys and message-signing across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BitClout (DeSo)
provider_slug: bitclout-deso
scheme_count: 3
schemes:
- description: Every DeSo account is an ed25519/secp256k1 keypair. The owner public key (Base58Check) identifies the account; the owner private key can sign any transaction and move funds.
  name: OwnerKeypair
  sources:
  - https://docs.deso.org/deso-identity/identity/concepts
  type: blockchain-keypair
- description: Apps request a derived key with a TransactionSpendingLimit that scopes which transaction types (and spend amounts) it may authorize. Users approve the limits once; the app then signs transactions on the user's behalf without ever touching the owner key.
  name: DerivedKey
  scope_object: TransactionSpendingLimitResponse
  sources:
  - https://docs.deso.org/deso-identity/identity/concepts
  - https://docs.deso.org/deso-backend/api
  type: scoped-signing-key
- description: The DeSo Identity Service (iframe + window API) hides key management, login, permission approval, and transaction signing behind a browser API so apps never handle raw private keys.
  name: Identity Service
  sources:
  - https://docs.deso.org/deso-identity/window-api/basics
  - https://docs.deso.org/deso-identity/iframe-api/basics
  type: signing-service
slug: bitclout-deso-authentication
source_filename: bitclout-deso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.deso.org/deso-identity/identity\ndocs: https://docs.deso.org/deso-identity/identity/concepts\nsummary:\n  model: blockchain-keypair\n  types:\n  - derived-keys\n  - message-signing\n  api_key_in: []\n  oauth2_flows: []\n  notes: DeSo does not use API keys, OAuth2, or bearer tokens. Data (read) endpoints\n    on a node are public and unauthenticated. Write operations are authenticated by\n    cryptographically signing transactions with the user's key material via the DeSo\n    Identity service.\nschemes:\n- name: OwnerKeypair\n  type: blockchain-keypair\n  description: Every DeSo account is an ed25519/secp256k1 keypair. The owner public\n    key (Base58Check) identifies the account; the owner private key can sign any transaction\n    and move funds.\n  sources:\n  - https://docs.deso.org/deso-identity/identity/concepts\n- name: DerivedKey\n  type: scoped-signing-key\n  description: Apps request a derived key with\
  \ a TransactionSpendingLimit that scopes\n    which transaction types (and spend amounts) it may authorize. Users approve the\n    limits once; the app then signs transactions on the user's behalf without ever\n    touching the owner key.\n  scope_object: TransactionSpendingLimitResponse\n  sources:\n  - https://docs.deso.org/deso-identity/identity/concepts\n  - https://docs.deso.org/deso-backend/api\n- name: Identity Service\n  type: signing-service\n  description: The DeSo Identity Service (iframe + window API) hides key management,\n    login, permission approval, and transaction signing behind a browser API so apps\n    never handle raw private keys.\n  sources:\n  - https://docs.deso.org/deso-identity/window-api/basics\n  - https://docs.deso.org/deso-identity/iframe-api/basics\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitclout-deso/refs/heads/main/authentication/bitclout-deso-authentication.yml
summary_line: derived-keys/message-signing · 3 schemes
tags:
- Company
- Crypto
- Blockchain
- Decentralized Social
- Web3
- Social Media
- NFT
- Creator Economy
---
