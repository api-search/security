---
api_key_in: []
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Mina Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mina Protocol secures its APIs with signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mina Protocol
provider_slug: mina-protocol
scheme_count: 2
schemes:
- algorithm: Schnorr signatures over the Pallas curve (Mina native)
  docs: https://docs.minaprotocol.com/mina-signer
  name: transaction-signature
  produced_by:
  - mina-signer (npm, o1-labs)
  - o1js (npm, o1-labs)
  - Rosetta offline signer CLI
  type: signature
- detail: GraphQL/Rosetta read endpoints are unauthenticated and bound to localhost:3085 (or an operator-firewalled host) by default; access control is a deployment concern for the node operator, not an API credential.
  name: node-endpoint-access
  type: network
slug: mina-protocol-authentication
source_filename: mina-protocol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.minaprotocol.com/mina-signer\nsummary:\n  types: [signature]\n  api_key: false\n  oauth2: false\n  detail: >-\n    Mina's node APIs (GraphQL, Rosetta) are not gated by API keys or OAuth.\n    Authorization for any state-changing operation is a cryptographic signature\n    over the transaction, using a Mina key pair (public + private key).\nschemes:\n  - name: transaction-signature\n    type: signature\n    algorithm: Schnorr signatures over the Pallas curve (Mina native)\n    produced_by:\n      - mina-signer (npm, o1-labs)\n      - o1js (npm, o1-labs)\n      - Rosetta offline signer CLI\n    docs: https://docs.minaprotocol.com/mina-signer\n  - name: node-endpoint-access\n    type: network\n    detail: >-\n      GraphQL/Rosetta read endpoints are unauthenticated and bound to\n      localhost:3085 (or an operator-firewalled host) by default; access control\n      is a deployment concern for the node operator, not\
  \ an API credential.\nnotes: >-\n  No OpenAPI securitySchemes exist in-repo to derive from; this profile is\n  searched from the provider docs. Key generation and signing are entirely\n  client-side.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mina-protocol/refs/heads/main/authentication/mina-protocol-authentication.yml
summary_line: signature · 2 schemes
tags:
- Company
- Crypto Web3
- Blockchain
- Zero Knowledge Proofs
- zk-SNARKs
- Smart Contracts
- GraphQL
- Rosetta API
- Developer Tools
---
