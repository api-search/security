---
api_key_in: []
api_specs:
- filename: seismic-systems-src20-factory-openapi.yml
  format: yaml
  label: Seismic
  slug: seismic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic-systems/refs/heads/main/openapi/seismic-systems-src20-factory-openapi.yml
auth_types:
- none
- wallet-signature
description: 'Seismic''s authentication model has two distinct layers. (1) The SRC20 Factory REST API is unauthenticated and read-only — it uses a public provider and holds no key. (2) On-chain interaction is authenticated cryptographically: writes are signed Seismic transactions (EIP-712 typed data, tx type 0x4A) and "signed reads" are authenticated eth_call requests that prove the caller''s identity to the contract, with calldata encrypted to the node''s TEE key via ECDH + AES-GCM. There is no OAuth, no API-key issuance, and no scopes surface.'
kind: authentication
layout: security
method: searched
name: Seismic Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seismic Systems secures its APIs with none and wallet-signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Seismic Systems
provider_slug: seismic-systems
scheme_count: 3
schemes:
- applies_to: openapi/seismic-systems-src20-factory-openapi.yml
  detail: The SRC20 Factory REST API requires no credentials and can only read public state.
  layer: rest-api
  name: rest-public
  type: none
- detail: Shielded writes are signed with the developer's wallet key and submitted via eth_sendRawTransaction; calldata is AES-GCM encrypted to the node TEE public key obtained through seismic_getTeePublicKey and an ECDH key exchange.
  layer: on-chain
  name: seismic-signed-transaction
  scheme: EIP-712 typed-data signature (Seismic tx type 0x4A)
  type: wallet-signature
- detail: Read calls that prove caller identity to the contract so a user can access their own shielded state (e.g. their SRC20 balance) without exposing it to others.
  layer: on-chain
  name: seismic-signed-read
  scheme: Authenticated eth_call (signed read)
  type: wallet-signature
slug: seismic-systems-authentication
source_filename: seismic-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.seismic.systems/reference/seismic-transaction/signed-reads.md\ndocs:\n  - https://docs.seismic.systems/reference/seismic-transaction.md\n  - https://docs.seismic.systems/reference/seismic-transaction/signed-reads.md\n  - https://docs.seismic.systems/getting-started/src20-factory/api.md\ndescription: >-\n  Seismic's authentication model has two distinct layers. (1) The SRC20 Factory\n  REST API is unauthenticated and read-only — it uses a public provider and holds\n  no key. (2) On-chain interaction is authenticated cryptographically: writes are\n  signed Seismic transactions (EIP-712 typed data, tx type 0x4A) and \"signed\n  reads\" are authenticated eth_call requests that prove the caller's identity to\n  the contract, with calldata encrypted to the node's TEE key via ECDH + AES-GCM.\n  There is no OAuth, no API-key issuance, and no scopes surface.\nsummary:\n  types: [none, wallet-signature]\n  rest_api_auth:\
  \ none\n  onchain_auth: [eip712-signed-transaction, signed-read, tee-ecdh-encryption]\n  oauth2_flows: []\nschemes:\n  - name: rest-public\n    layer: rest-api\n    type: none\n    applies_to: openapi/seismic-systems-src20-factory-openapi.yml\n    detail: The SRC20 Factory REST API requires no credentials and can only read public state.\n  - name: seismic-signed-transaction\n    layer: on-chain\n    type: wallet-signature\n    scheme: EIP-712 typed-data signature (Seismic tx type 0x4A)\n    detail: >-\n      Shielded writes are signed with the developer's wallet key and submitted via\n      eth_sendRawTransaction; calldata is AES-GCM encrypted to the node TEE public key\n      obtained through seismic_getTeePublicKey and an ECDH key exchange.\n  - name: seismic-signed-read\n    layer: on-chain\n    type: wallet-signature\n    scheme: Authenticated eth_call (signed read)\n    detail: >-\n      Read calls that prove caller identity to the contract so a user can access their own\n      shielded\
  \ state (e.g. their SRC20 balance) without exposing it to others.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seismic-systems/refs/heads/main/authentication/seismic-systems-authentication.yml
summary_line: none/wallet-signature · 3 schemes
tags:
- Company
- Blockchain
- Privacy
- Encryption
- Stablecoins
- Fintech
- Web3
- Smart Contracts
- EVM
- Cryptography
- Developer Tools
---
