---
api_key_in: []
auth_types:
- web3-signature
description: ''
kind: authentication
layout: security
method: searched
name: Sunscreen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sunscreen secures its APIs with web3-signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sunscreen
provider_slug: sunscreen
scheme_count: 1
schemes:
- key_format: 0x-prefixed Ethereum private key
  modes:
  - detail: Backend/application server holds the signing key and signs on behalf of users.
    name: web2
  - detail: User's wallet signs requests directly (browser demo shows both modes).
    name: web3
  name: PrivateKeySigner
  scheme: ecdsa-secp256k1
  sources:
  - spf-client README
  - spf-docs.sunscreen.tech
  type: web3-signature
slug: sunscreen-authentication
source_filename: sunscreen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/Sunscreen-tech/spf-client (README.md) + https://spf-docs.sunscreen.tech/docs/service\nsummary:\n  types: [web3-signature]\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  The Sunscreen SPF service does not use API keys or OAuth. Requests to the SPF\n  testnet REST service are authenticated with an Ethereum-style signature: the\n  client signs with a private key (a `PrivateKeySigner` holding a `0x...` key in\n  the TypeScript SDK, or `--private-key 0x...` on the Rust CLI). On-chain access\n  control (ACL) then governs which addresses may decrypt or run against a given\n  ciphertext. A \"web2\" mode lets an application server hold the signing key on\n  behalf of users; a \"web3\" mode signs directly from the user's wallet.\nschemes:\n  - name: PrivateKeySigner\n    type: web3-signature\n    scheme: ecdsa-secp256k1\n    key_format: \"0x-prefixed Ethereum private key\"\n    sources: [spf-client README, spf-docs.sunscreen.tech]\n\
  \    modes:\n      - name: web2\n        detail: Backend/application server holds the signing key and signs on behalf of users.\n      - name: web3\n        detail: User's wallet signs requests directly (browser demo shows both modes).\nauthorization:\n  model: on-chain-acl\n  detail: Ciphertext access (admin / decrypt / run) is granted per-address and checked via the SPF smart-contract ACL.\ndocs: https://spf-docs.sunscreen.tech/docs/acl\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunscreen/refs/heads/main/authentication/sunscreen-authentication.yml
summary_line: web3-signature · 1 scheme
tags:
- Company
- Infra Devtools
- Fully Homomorphic Encryption
- Cryptography
- Blockchain
- Web3
- Privacy
- Developer Tools
- FHE
---
