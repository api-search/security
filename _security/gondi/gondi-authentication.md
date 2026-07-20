---
api_key_in:
- header
auth_types:
- siwe
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gondi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gondi secures its APIs with siwe and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gondi
provider_slug: gondi
scheme_count: 2
schemes:
- flow: Call the generateSignInNonce mutation to obtain a nonce, construct and sign the SIWE message with the connected wallet, then call signInWithEthereum with the signature to establish an authenticated session.
  name: SignInWithEthereum
  operations:
  - generateSignInNonce
  - signInWithEthereum
  sources:
  - graphql/gondi-schema.graphql
  standard: EIP-4361
  type: siwe
- flow: An authenticated user mints a programmatic API key via the createApiKey mutation for server-to-server access to the GraphQL API.
  in: header
  minted_by: createApiKey
  name: ApiKey
  operations:
  - createApiKey
  sources:
  - graphql/gondi-schema.graphql
  type: apiKey
slug: gondi-authentication
source_filename: gondi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.gondi.xyz/graphql\ndocs: https://github.com/gondixyz/gondi-js\nsummary:\n  types: [siwe, apiKey]\n  api_key_in: [header]\n  notes: >-\n    Gondi's off-chain GraphQL API authenticates users with Sign-In With Ethereum\n    (EIP-4361) sessions and issues programmatic API keys. There are no OAuth2\n    scopes; authorization to move value is enforced on-chain via wallet\n    signatures, not server-side scopes.\nschemes:\n  - name: SignInWithEthereum\n    type: siwe\n    standard: EIP-4361\n    flow: >-\n      Call the generateSignInNonce mutation to obtain a nonce, construct and sign\n      the SIWE message with the connected wallet, then call signInWithEthereum\n      with the signature to establish an authenticated session.\n    operations: [generateSignInNonce, signInWithEthereum]\n    sources: [graphql/gondi-schema.graphql]\n  - name: ApiKey\n    type: apiKey\n    in: header\n    minted_by: createApiKey\n    flow:\
  \ >-\n      An authenticated user mints a programmatic API key via the createApiKey\n      mutation for server-to-server access to the GraphQL API.\n    operations: [createApiKey]\n    sources: [graphql/gondi-schema.graphql]\nsigning:\n  model: non-custodial\n  notes: >-\n    Loan offers, collection offers, and renegotiation offers are signed\n    client-side with the user's wallet (generate*OfferToBeSigned returns the\n    payload to sign; saveSigned* persists the signature). The API never holds\n    keys or moves funds without a wallet signature.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gondi/refs/heads/main/authentication/gondi-authentication.yml
summary_line: siwe/apiKey · 2 schemes
tags:
- Company
- Crypto
- NFT
- DeFi
- Lending
- NFT Finance
- GraphQL
- Web3
---
