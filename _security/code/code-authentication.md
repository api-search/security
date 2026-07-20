---
api_key_in: []
auth_types:
- self-custodial-keypair
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: Code Authentication
name_suffix: Authentication
oauth_flows: []
overview: Code secures its APIs with self-custodial-keypair and jwt across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Code
provider_slug: code
scheme_count: 2
schemes:
- description: Clients sign gRPC requests (intents, swaps, messages) with an Ed25519 keypair derived from the user's self-custodial wallet. No account registration, API key, or OAuth token is required ("no sign-up necessary"). Timelock accounts on Solana enforce ownership on-chain.
  name: Ed25519 request signing
  sources:
  - grpc/code-transaction-v2.proto
  - grpc/code-common-v1.proto
  type: self-custodial-keypair
- description: Server-side payment-event webhooks are delivered as JWT-signed notifications; the receiving server verifies the JWT signature to confirm the event originated from Code and was not tampered with.
  name: Webhook JWT verification
  sources:
  - asyncapi/code-webhooks.yml
  type: jwt
slug: code-authentication
source_filename: code-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://code-payments.github.io/code-sdk/docs/\ndocs: https://code-payments.github.io/code-sdk/docs/guide/introduction.html\nnote: >-\n  Code exposes a gRPC/Protobuf API (code-protobuf-api), not a REST API, so there\n  is no OpenAPI securityScheme to derive from. Authentication is self-custodial\n  and protocol-level rather than API-key/OAuth based.\nsummary:\n  types: [self-custodial-keypair, jwt]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: Ed25519 request signing\n    type: self-custodial-keypair\n    description: >-\n      Clients sign gRPC requests (intents, swaps, messages) with an Ed25519\n      keypair derived from the user's self-custodial wallet. No account\n      registration, API key, or OAuth token is required (\"no sign-up\n      necessary\"). Timelock accounts on Solana enforce ownership on-chain.\n    sources: [grpc/code-transaction-v2.proto, grpc/code-common-v1.proto]\n  - name: Webhook JWT verification\n\
  \    type: jwt\n    description: >-\n      Server-side payment-event webhooks are delivered as JWT-signed\n      notifications; the receiving server verifies the JWT signature to confirm\n      the event originated from Code and was not tampered with.\n    sources: [asyncapi/code-webhooks.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code/refs/heads/main/authentication/code-authentication.yml
summary_line: self-custodial-keypair/jwt · 2 schemes
tags:
- Company
- Payments
- Micropayments
- Wallet
- Solana
- Blockchain
- Cryptocurrency
- gRPC
- Self-Custodial
---
