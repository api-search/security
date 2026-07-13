---
api_key_in: []
api_specs:
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Identity & KYC/KYB API
  slug: sila-money-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Wallets API
  slug: sila-money-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Bank Accounts API
  slug: sila-money-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Payments & Transactions API
  slug: sila-money-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Payment Methods & Cards API
  slug: sila-money-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: documented
name: Sila Money Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sila secures its APIs with signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sila
provider_slug: sila-money
scheme_count: 3
schemes:
- algorithm: ECDSA
  curve: secp256k1
  description: Hex-encoded ECDSA (secp256k1) signature over a Keccak-256 (SHA3) hash of the stringified JSON message body, signed with the application's private key. Sent in the "authsignature" request header. Sila stores only addresses (derived from public keys); private keys never leave the client. Confirmed live - a POST to /0.2/check_handle with no signature header returns HTTP 400 with validation_details.header "This field is required."
  hash: Keccak-256
  in: header
  name: authsignature
  scope: application
  sources:
  - https://docs.silamoney.com/docs/ecdsa-overview
  type: signature
- algorithm: ECDSA
  curve: secp256k1
  description: Second ECDSA signature over the same message hash, signed with the end user's registered keypair (from /register or /register_wallet). Required in addition to authsignature on user-scoped endpoints (link_account, issue_sila, transfer_sila, redeem_sila, get_transactions, etc.). Sent in the "usersignature" header.
  hash: Keccak-256
  in: header
  name: usersignature
  scope: user
  sources:
  - https://docs.silamoney.com/docs/ecdsa-overview
  type: signature
- algorithm: ECDSA
  curve: secp256k1
  description: Third ECDSA signature signed with a registered business keypair, used alongside authsignature (and usersignature) for KYB / business-entity operations. Sent in the "businesssignature" header. The precise set of endpoints that require it is not exhaustively enumerated in the pages reviewed.
  hash: Keccak-256
  in: header
  name: businesssignature
  scope: business
  sources:
  - https://docs.silamoney.com/docs/ecdsa-overview
  type: signature
slug: sila-money-authentication
source_filename: sila-money-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://docs.silamoney.com/docs/ecdsa-overview\nsummary:\n  types:\n  - signature\nschemes:\n- name: authsignature\n  type: signature\n  algorithm: ECDSA\n  curve: secp256k1\n  hash: Keccak-256\n  in: header\n  scope: application\n  description: >-\n    Hex-encoded ECDSA (secp256k1) signature over a Keccak-256 (SHA3) hash of the\n    stringified JSON message body, signed with the application's private key.\n    Sent in the \"authsignature\" request header. Sila stores only addresses\n    (derived from public keys); private keys never leave the client. Confirmed\n    live - a POST to /0.2/check_handle with no signature header returns HTTP 400\n    with validation_details.header \"This field is required.\"\n  sources:\n  - https://docs.silamoney.com/docs/ecdsa-overview\n- name: usersignature\n  type: signature\n  algorithm: ECDSA\n  curve: secp256k1\n  hash: Keccak-256\n  in: header\n  scope: user\n  description: >-\n    Second\
  \ ECDSA signature over the same message hash, signed with the end\n    user's registered keypair (from /register or /register_wallet). Required in\n    addition to authsignature on user-scoped endpoints (link_account, issue_sila,\n    transfer_sila, redeem_sila, get_transactions, etc.). Sent in the\n    \"usersignature\" header.\n  sources:\n  - https://docs.silamoney.com/docs/ecdsa-overview\n- name: businesssignature\n  type: signature\n  algorithm: ECDSA\n  curve: secp256k1\n  hash: Keccak-256\n  in: header\n  scope: business\n  description: >-\n    Third ECDSA signature signed with a registered business keypair, used\n    alongside authsignature (and usersignature) for KYB / business-entity\n    operations. Sent in the \"businesssignature\" header. The precise set of\n    endpoints that require it is not exhaustively enumerated in the pages\n    reviewed.\n  sources:\n  - https://docs.silamoney.com/docs/ecdsa-overview\nnotes: >-\n  Sila uses no bearer token or API key in the classic\
  \ sense - authentication is\n  request signing. Because standard tooling (Postman, generic OpenAPI clients)\n  cannot compute a per-body ECDSA signature, Sila publishes helper tooling:\n  sila-postman-signer (a local signing proxy) and language SDKs\n  (JavaScript, Python, Java, PHP, C#) at https://github.com/sila-Money. Private\n  keys are hex-encoded 64-character strings (no 0x prefix). An \"app handle\" plus\n  its address is provisioned per application in the Sila console.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/authentication/sila-money-authentication.yml
summary_line: signature · 3 schemes
tags:
- Embedded Finance
- Banking as a Service
- Payments
- Digital Wallet
- ACH
- KYC
- KYB
- Money Transfer
- Fintech
- Banking API
- Virtual Accounts
---
