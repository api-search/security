---
api_key_in: []
auth_types:
- none
- signed-message
description: 'Authentication / authorization model for the Farcaster / Snapchain developer surface. Derived from the Snapchain HTTP API reference and the Farcaster message protobuf (signature scheme, signer, key registry). There are no HTTP API keys, bearer tokens, or OAuth flows on the node HTTP API: reads are open and writes are authorized by cryptographic message signatures.'
kind: authentication
layout: security
method: searched
name: Merkle Manufactory Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Merkle Manufactory Inc. secures its APIs with none and signed-message across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Merkle Manufactory Inc.
provider_slug: merkle-manufactory-inc
scheme_count: 2
schemes:
- applies_to: All GET endpoints of the Snapchain HTTP API (/v1/*)
  detail: Read endpoints on a Snapchain node are unauthenticated. Clients query a public node directly with no credential.
  name: PublicRead
  type: none
- applies_to: POST /v1/submitMessage
  detail: Writes are authorized by an Ed25519 signature over the message hash, produced by an account key (signer) that the user has registered on-chain via the Farcaster Key Registry. The submitted protobuf Message carries the fid, signer public key, hash, and signature; the node verifies the signer is an authorized key for that fid before merging.
  keys_registered_via: Farcaster Key Registry (on-chain, Optimism)
  name: SignedMessageWrite
  signature_scheme: SIGNATURE_SCHEME_ED25519
  type: message-signature
slug: merkle-manufactory-inc-authentication
source_filename: merkle-manufactory-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://snapchain.farcaster.xyz/reference/httpapi/message\ndescription: >-\n  Authentication / authorization model for the Farcaster / Snapchain developer\n  surface. Derived from the Snapchain HTTP API reference and the Farcaster\n  message protobuf (signature scheme, signer, key registry). There are no HTTP\n  API keys, bearer tokens, or OAuth flows on the node HTTP API: reads are open\n  and writes are authorized by cryptographic message signatures.\nsummary:\n  types:\n    - none\n    - signed-message\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: PublicRead\n    type: none\n    applies_to: All GET endpoints of the Snapchain HTTP API (/v1/*)\n    detail: >-\n      Read endpoints on a Snapchain node are unauthenticated. Clients query a\n      public node directly with no credential.\n  - name: SignedMessageWrite\n    type: message-signature\n    applies_to: POST /v1/submitMessage\n    signature_scheme: SIGNATURE_SCHEME_ED25519\n\
  \    detail: >-\n      Writes are authorized by an Ed25519 signature over the message hash,\n      produced by an account key (signer) that the user has registered on-chain\n      via the Farcaster Key Registry. The submitted protobuf Message carries the\n      fid, signer public key, hash, and signature; the node verifies the signer\n      is an authorized key for that fid before merging.\n    keys_registered_via: Farcaster Key Registry (on-chain, Optimism)\nidentity:\n  siwf:\n    name: Sign In with Farcaster (SIWF)\n    docs: https://docs.farcaster.xyz/developers/siwf\n    detail: >-\n      Application-level authentication standard (an EIP-4361 Sign-In-with-\n      Ethereum profile) that lets third-party apps authenticate a Farcaster user\n      and read their identity. Implemented client-side via AuthKit.\n    authkit: https://docs.farcaster.xyz/auth-kit/installation\nnotes: >-\n  This provider publishes no OpenAPI, so this profile is captured from the\n  human-readable HTTP API reference\
  \ and the protobuf definitions in\n  grpc/ rather than derived from securitySchemes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merkle-manufactory-inc/refs/heads/main/authentication/merkle-manufactory-inc-authentication.yml
summary_line: none/signed-message · 2 schemes
tags:
- Company
- Social
- Decentralized Social
- Protocol
- Blockchain
- Web3
- Developer Platform
- Farcaster
---
