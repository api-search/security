---
api_key_in: []
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Succinct Authentication
name_suffix: Authentication
oauth_flows: []
overview: Succinct secures its APIs with signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Succinct
provider_slug: succinct
scheme_count: 2
schemes:
- description: Requester/prover account key pair. Generate with `cast wallet new` (Foundry) or export from a wallet. The private key is set as NETWORK_PRIVATE_KEY and used by ProverClient to sign gRPC calls (RequestProof, FulfillProof, etc.). Fund the derived account with PROVE deposited via the Explorer before requesting proofs.
  docs: https://docs.succinct.xyz/docs/sp1/prover-network/quickstart
  env: NETWORK_PRIVATE_KEY
  location: request-signature
  name: NetworkKeyPair
  scheme: secp256k1
  type: signature
- description: The Verifier gRPC service (VerifyProof) requires no authentication — proofs are self-verifying.
  name: VerifierPublic
  type: none
slug: succinct-authentication
source_filename: succinct-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.succinct.xyz/docs/sp1/prover-network/quickstart\nnotes: >-\n  Succinct has no REST/OpenAPI surface; its programmatic API is the gRPC Succinct\n  Prover Network (see grpc/). Authentication is not API-key or OAuth based — the\n  network authenticates requesters and provers with Secp256k1 key pairs (the same\n  key primitive as Ethereum wallets). Requests to the ProverNetwork gRPC service\n  are signed with the account private key; the assigned fulfiller/requester\n  identity is derived from the signature.\nsummary:\n  types: [signature]\n  scheme: secp256k1-signed-grpc\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: NetworkKeyPair\n    type: signature\n    scheme: secp256k1\n    location: request-signature\n    env: NETWORK_PRIVATE_KEY\n    docs: https://docs.succinct.xyz/docs/sp1/prover-network/quickstart\n    description: >-\n      Requester/prover account key pair. Generate with `cast wallet new` (Foundry)\n\
  \      or export from a wallet. The private key is set as NETWORK_PRIVATE_KEY and\n      used by ProverClient to sign gRPC calls (RequestProof, FulfillProof, etc.).\n      Fund the derived account with PROVE deposited via the Explorer before\n      requesting proofs.\n  - name: VerifierPublic\n    type: none\n    description: >-\n      The Verifier gRPC service (VerifyProof) requires no authentication — proofs\n      are self-verifying.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/succinct/refs/heads/main/authentication/succinct-authentication.yml
summary_line: signature · 2 schemes
tags:
- Company
- Crypto Infrastructure
- Zero-Knowledge Proofs
- zkVM
- Blockchain
- Ethereum
- Cryptography
- Developer Tools
- Prover Network
- gRPC
---
