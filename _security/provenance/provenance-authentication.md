---
api_key_in: []
auth_types:
- none-for-reads
- signature-based-for-writes
description: ''
kind: authentication
layout: security
method: searched
name: Provenance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Provenance secures its APIs with none-for-reads and signature-based-for-writes across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Provenance
provider_slug: provenance
scheme_count: 2
schemes:
- applies_to: All Query (read) operations over REST (api.provenance.io), gRPC, and RPC.
  name: PublicQuery
  note: Chain state is public; no credentials required to read.
  type: none
- algorithm: secp256k1
  applies_to: All Msg (write) operations that broadcast transactions.
  name: TransactionSignature
  note: State-changing transactions are signed by the sending account's private key (secp256k1) and validated by consensus using the account's public key, sequence (nonce), and chain-id. Granular delegation is available via the Cosmos authz and feegrant modules and Provenance marker access grants.
  type: signature
slug: provenance-authentication
source_filename: provenance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  docs.provenance.io + Cosmos SDK transaction model (grpc/*.proto Msg services). No\n  OpenAPI securitySchemes exist; the auth model is the Cosmos public-chain model.\nsummary:\n  types: [none-for-reads, signature-based-for-writes]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: PublicQuery\n  type: none\n  applies_to: All Query (read) operations over REST (api.provenance.io), gRPC, and RPC.\n  note: Chain state is public; no credentials required to read.\n- name: TransactionSignature\n  type: signature\n  algorithm: secp256k1\n  applies_to: All Msg (write) operations that broadcast transactions.\n  note: >-\n    State-changing transactions are signed by the sending account's private key\n    (secp256k1) and validated by consensus using the account's public key, sequence\n    (nonce), and chain-id. Granular delegation is available via the Cosmos authz and\n    feegrant modules and Provenance marker access grants.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provenance/refs/heads/main/authentication/provenance-authentication.yml
summary_line: none-for-reads/signature-based-for-writes · 2 schemes
tags:
- Company
- Blockchain
- Financial Services
- Tokenization
- Real-World Assets
- Cosmos SDK
- gRPC
- Web3
- DeFi
- Digital Assets
---
