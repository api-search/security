---
api_key_in: []
auth_types: []
description: There is no transport-level authentication scheme. Authorization is cryptographic and lives inside the transaction.
kind: authentication
layout: security
method: derived
name: Topl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Topl declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Topl
provider_slug: topl
scheme_count: 0
schemes: []
slug: topl-authentication
source_filename: topl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource: >-\n  Derived from grpc/ (the verbatim protobuf contract) and from the archived BramblDart SDK\n  documentation in github.com/Topl/Knowledge-Base\n  (docs/Developers/06-Software Development Kits/01-BramblDart.md). The derive-authentication.py\n  helper was not used: it reads OpenAPI securitySchemes and this provider publishes a protobuf\n  contract, not an OpenAPI.\nname: Topl / Apparatus authentication profile\ndescription: >-\n  There is no transport-level authentication scheme. Authorization is cryptographic and lives\n  inside the transaction.\ntransport_auth:\n  schemes: []\n  note: >-\n    No apiKey, http, oauth2, openIdConnect or mutualTLS scheme is declared anywhere in the 38\n    published proto files, and no reachable Topl document describes obtaining an API\n    credential. The documented public testnet endpoint accepted TLS-encrypted but\n    unauthenticated gRPC calls.\ntransaction_authorization:\n  model: Quivr\
  \ propositions and proofs\n  description: >-\n    Every transaction output is locked by a Proposition and spent by supplying a matching\n    Proof, carried in an Attestation. This is the real access control in the system: reads are\n    open, writes are gated by possession of a key that satisfies the lock.\n  contract_locations:\n  - grpc/quivr/models/proposition.proto\n  - grpc/quivr/models/proof.proto\n  - grpc/brambl/models/box/attestation.proto\n  - grpc/brambl/models/box/lock.proto\n  - grpc/brambl/models/box/challenge.proto\nkey_material:\n  signing: Extended Ed25519 signing keys\n  derivation: HD wallet derivation supported by the SDKs\n  keystore: 'v1 encrypted key files, password-protected'\n  source: >-\n    github.com/Topl/Knowledge-Base docs/Developers/06-Software Development Kits/01-BramblDart.md\n    — \"The library supports raw private keys and v1 encrypted key-files. In addition, it also\n    supports the generation of keys via a HD wallet.\"\n  wallet_tooling: 'brambl-cli\
  \ wallet (initialize-wallet, current-address, balance) — see cli/topl-cli.yml'\nscopes:\n  published: false\n  note: >-\n    No OAuth scopes exist, so scopes/ is deliberately absent. derive-oauth-scopes.py was not\n    run: there is no oauth2 securityScheme and no OAuth documentation to derive from.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topl/refs/heads/main/authentication/topl-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Blockchain
- Distributed Ledger
- gRPC
- Protobuf
- Web3
- Proof of Stake
- Sustainability
- Impact
- Tokenization
- Wound Down
---
