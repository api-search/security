---
api_key_in: []
auth_types:
- signature
- network-partition
- transport-encryption
description: ''
kind: authentication
layout: security
method: searched
name: Bitfury Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: BitFury secures its APIs with signature, network-partition, and transport-encryption across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BitFury
provider_slug: bitfury-group
scheme_count: 4
schemes:
- algorithm: Ed25519
  applies_to: write operations (transactions submitted over REST or WebSocket)
  description: Transactions are authenticated by an Ed25519 digital signature carried in the JSON serialization of the transaction, not by an HTTP credential. The caller is identified by the transaction author's public key, by a calling service instance ID, or by the blockchain itself (see exonum.runtime.Caller in grpc/bitfury-group-exonum-runtime-auth.proto).
  name: ed25519-transaction-signature
  source: grpc/bitfury-group-exonum-runtime-auth.proto
  type: signature
- applies_to: read operations on the public HTTP server
  description: 'GET endpoints defined by services on the public HTTP server are generally not authenticated. Integrity is provided by Merkle proofs rather than by access control: a light client can verify that a response was authorized by a supermajority of validators.'
  name: unauthenticated-public-read
  type: none
- applies_to: administrative operations (system API plugin, supervisor private endpoints)
  description: The Rust runtime runs two HTTP servers, public and private, with separate endpoint sets and separate ports. Privileged operations - node info/stats/peers/consensus status/shutdown, artifact deployment, config proposals - are only wired onto the private server, which the operator is expected to keep off the public network. There is no token or key scheme on these endpoints; access control is the deployment's responsibility.
  name: private-http-server
  type: network-partition
- applies_to: full-node to full-node connections
  description: All peer-to-peer connections between full nodes are encrypted with the Noise Protocol, and every full node is authenticated with public-key cryptography.
  name: noise-protocol-p2p
  type: transport-encryption
slug: bitfury-group-authentication
source_filename: bitfury-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://exonum.com/doc/version/latest/advanced/network/\ndocs:\n- https://exonum.com/doc/version/latest/advanced/network/\n- https://exonum.com/doc/version/latest/architecture/transactions/\n- https://exonum.com/doc/version/latest/architecture/clients/\nnote: 'Derived mechanically first with 0-working/derive-authentication.py, which found no OpenAPI\n  securitySchemes because Bitfury publishes no OpenAPI for Exonum. The profile below is read from the\n  published Exonum documentation and source, and describes the framework''s actual authorization model\n  rather than an HTTP securityScheme list.'\nsummary:\n  types: [signature, network-partition, transport-encryption]\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  bearer_tokens: false\nschemes:\n- name: ed25519-transaction-signature\n  type: signature\n  algorithm: Ed25519\n  applies_to: write operations (transactions\
  \ submitted over REST or WebSocket)\n  description: 'Transactions are authenticated by an Ed25519 digital signature carried in the JSON\n    serialization of the transaction, not by an HTTP credential. The caller is identified by the\n    transaction author''s public key, by a calling service instance ID, or by the blockchain itself\n    (see exonum.runtime.Caller in grpc/bitfury-group-exonum-runtime-auth.proto).'\n  source: grpc/bitfury-group-exonum-runtime-auth.proto\n- name: unauthenticated-public-read\n  type: none\n  applies_to: read operations on the public HTTP server\n  description: 'GET endpoints defined by services on the public HTTP server are generally not\n    authenticated. Integrity is provided by Merkle proofs rather than by access control: a light client\n    can verify that a response was authorized by a supermajority of validators.'\n- name: private-http-server\n  type: network-partition\n  applies_to: administrative operations (system API plugin, supervisor private\
  \ endpoints)\n  description: 'The Rust runtime runs two HTTP servers, public and private, with separate endpoint sets\n    and separate ports. Privileged operations - node info/stats/peers/consensus status/shutdown, artifact\n    deployment, config proposals - are only wired onto the private server, which the operator is expected\n    to keep off the public network. There is no token or key scheme on these endpoints; access control is\n    the deployment''s responsibility.'\n- name: noise-protocol-p2p\n  type: transport-encryption\n  applies_to: full-node to full-node connections\n  description: All peer-to-peer connections between full nodes are encrypted with the Noise Protocol, and\n    every full node is authenticated with public-key cryptography.\ngaps:\n- No OAuth 2.0, OpenID Connect, API key or bearer-token scheme exists anywhere in the Exonum HTTP surface.\n- Authorization of the private HTTP server is delegated entirely to network placement, so an operator who\n  exposes it inherits\
  \ an unauthenticated administrative API.\nx-evidence:\n  fetched: '2026-07-31'\n  source_files:\n  - https://github.com/exonum/exonum/blob/master/components/system-api/src/private.rs\n  - https://github.com/exonum/exonum-proto-sources/blob/master/src/exonum/runtime/auth.proto\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitfury-group/refs/heads/main/authentication/bitfury-group-authentication.yml
summary_line: signature/network-partition/transport-encryption · 4 schemes
tags:
- Company
- Blockchain
- Bitcoin
- Cryptocurrency
- Distributed Ledger
- Permissioned Blockchain
- Open Source
- Data Centers
- Mining Hardware
- Enterprise Blockchain
---
