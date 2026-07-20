---
api_key_in: []
api_specs:
- filename: filament-orderbook-asyncapi.yml
  format: yaml
  label: Filament API
  slug: filament-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/filament/refs/heads/main/asyncapi/filament-orderbook-asyncapi.yml
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Filament Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filament secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Filament
provider_slug: filament
scheme_count: 1
schemes:
- algorithm: EIP-191 personal_sign (ethers.js Wallet.signMessage)
  applies_to:
  - POST /filament/api/v1/exchange
  - updateIsolatedMargin payloads
  - cancel payloads
  description: 'Every mutating request (place/cancel order, update isolated margin) carries a `signature` field produced by signing the order''s `orderId` with the trader''s private key: `signer.signMessage(orderId)`. The `account` field must be the signer''s wallet address in lowercase. Order ids are generated with `nanoid().toLowerCase()`. There is no bearer token, API key header, or session — authenticity is proven per-order by the signature.'
  identity_field: account
  library: ethers.js v5.7.2
  name: WalletSignature
  signed_payload_field: orderId
  type: signature
slug: filament-authentication
source_filename: filament-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.filament.finance/market-makers/filament-api\ndocs: https://docs.filament.finance/market-makers/filament-api\nsummary:\n  types:\n  - signature\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Filament uses wallet-signature authentication rather than API keys or OAuth.\n    There are no securitySchemes because the API is not described by an OpenAPI\n    document; the scheme below is captured from the published API documentation.\nschemes:\n- name: WalletSignature\n  type: signature\n  algorithm: EIP-191 personal_sign (ethers.js Wallet.signMessage)\n  library: ethers.js v5.7.2\n  description: >-\n    Every mutating request (place/cancel order, update isolated margin) carries a\n    `signature` field produced by signing the order's `orderId` with the trader's\n    private key: `signer.signMessage(orderId)`. The `account` field must be the\n    signer's wallet address in lowercase. Order ids are generated with\n\
  \    `nanoid().toLowerCase()`. There is no bearer token, API key header, or\n    session — authenticity is proven per-order by the signature.\n  signed_payload_field: orderId\n  identity_field: account\n  applies_to:\n  - POST /filament/api/v1/exchange\n  - updateIsolatedMargin payloads\n  - cancel payloads\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filament/refs/heads/main/authentication/filament-authentication.yml
summary_line: signature · 1 scheme
tags:
- Company
- Crypto
- DeFi
- Derivatives
- Perpetuals
- DEX
- Trading
- Blockchain
- Sei
- Web3
---
