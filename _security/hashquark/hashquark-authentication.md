---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hashquark Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashKey Cloud (HashQuark) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HashKey Cloud (HashQuark)
provider_slug: hashquark
scheme_count: 1
schemes:
- authorization_format: Quark-Keccak256-ECDSA Address={address},Nonce={uuid},Timestamp={unixSeconds},Signature={hex}
  header: Authorization
  in: header
  name: Quark-Keccak256-ECDSA
  replay_protection:
  - per-request UUID nonce
  - unix timestamp
  scheme: signature
  signature:
    algorithm: ECDSA (Ethereum crypto.Sign over the Keccak256 digest)
    curve: secp256k1
    hash: keccak256
    key: client Ethereum private key (address registered with the broker)
    message: keccak256(nonce_bytes || bigEndian32(timestamp))
  sources:
  - packages/hashquark-packages.yml
  - https://github.com/hashquark-staking/staking-service-sdk
  type: http
slug: hashquark-authentication
source_filename: hashquark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/hashquark-staking/staking-service-sdk (staking_service/init.go, sign.go)\ndocs: https://hashkeycloud.gitbook.io/docs/api/staking-api/get-started\nsummary:\n  types:\n  - http\n  scheme: signature\n  description: >-\n    HashKey Cloud (HashQuark) staking-service requests are authenticated with a\n    custom request-signature scheme rather than API keys or OAuth. Each request\n    carries an Authorization header of the form\n    \"Quark-Keccak256-ECDSA Address=<address>,Nonce=<uuid>,Timestamp=<unix>,Signature=<hex>\".\nschemes:\n- name: Quark-Keccak256-ECDSA\n  type: http\n  scheme: signature\n  in: header\n  header: Authorization\n  authorization_format: >-\n    Quark-Keccak256-ECDSA Address={address},Nonce={uuid},Timestamp={unixSeconds},Signature={hex}\n  signature:\n    curve: secp256k1\n    hash: keccak256\n    message: keccak256(nonce_bytes || bigEndian32(timestamp))\n    algorithm: ECDSA (Ethereum crypto.Sign\
  \ over the Keccak256 digest)\n    key: client Ethereum private key (address registered with the broker)\n  replay_protection:\n  - per-request UUID nonce\n  - unix timestamp\n  sources:\n  - packages/hashquark-packages.yml\n  - https://github.com/hashquark-staking/staking-service-sdk\nnotes: >-\n  No OAuth2/OIDC or apiKey security scheme is published; the account/broker\n  address and its Ethereum keypair are the credential. Base URL is provisioned\n  per broker and injected into the SDK (no fixed public host).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashquark/refs/heads/main/authentication/hashquark-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Blockchain
- Staking
- Web3
- Validators
- Cryptocurrency
- Node Infrastructure
- Proof of Stake
- Ethereum
- DeFi
---
