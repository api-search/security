---
api_key_in:
- query
api_specs:
- filename: unlock-protocol-locksmith-openapi.yml
  format: yaml
  label: Unlock Locksmith API
  slug: unlock-locksmith-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock-protocol/refs/heads/main/openapi/unlock-protocol-locksmith-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Unlock Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unlock Protocol secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unlock Protocol
provider_slug: unlock-protocol
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: User
  note: Obtained via SIWE login; short expiry, renewed with a refresh token (revoke and logout operations invalidate tokens).
  scheme: bearer
  sources:
  - openapi/unlock-protocol-locksmith-openapi.yml
  type: http
- in: query
  name: Application
  note: Issued per application (createApplication operation); listed/rotated via the applications operations.
  parameter: api-key
  sources:
  - openapi/unlock-protocol-locksmith-openapi.yml
  type: apiKey
slug: unlock-protocol-authentication
source_filename: unlock-protocol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unlock-protocol-locksmith-openapi.yml\ndocs: https://docs.unlock-protocol.com/tools/locksmith/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  model: >-\n    Sign-In with Ethereum (EIP-4361): the client fetches a nonce (nonce operation), signs a SIWE\n    message with the user's wallet, and posts it to the login operation. Locksmith verifies the\n    signature and issues a short-lived JWT access token (sent as Authorization bearer) plus a\n    refresh token for renewal. Applications can alternatively authenticate with an api-key query\n    parameter issued per registered application. Users without wallets can use Unlock Accounts\n    (email/Google) via the same flow; a Privy-based login (loginWithPrivy) is also exposed.\n  siwe_docs: https://docs.unlock-protocol.com/tools/sign-in-with-ethereum/\n  sdk_helper: LocksmithService.createSiweMessage in @unlock-protocol/unlock-js\nschemes:\n- name: User\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  note: Obtained via SIWE login; short expiry, renewed with a refresh token (revoke and logout operations invalidate tokens).\n  sources:\n  - openapi/unlock-protocol-locksmith-openapi.yml\n- name: Application\n  type: apiKey\n  in: query\n  parameter: api-key\n  note: Issued per application (createApplication operation); listed/rotated via the applications operations.\n  sources:\n  - openapi/unlock-protocol-locksmith-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unlock-protocol/refs/heads/main/authentication/unlock-protocol-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Blockchain
- Memberships
- Subscriptions
- NFT
- Ticketing
- Web3
- Payments
---
