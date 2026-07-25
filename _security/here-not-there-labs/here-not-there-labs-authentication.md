---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Here Not There Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Here Not There Labs declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Here Not There Labs
provider_slug: here-not-there-labs
scheme_count: 5
schemes:
- description: Users sign a SIWE message with their Ethereum wallet to establish identity. Implemented via the first-party @towns-protocol siwe library.
  evidence: siwe package published by the org; connectTowns / signAndConnect react hooks.
  id: siwe
  standard: EIP-4361 (Sign-In with Ethereum)
  type: wallet-signature
- description: A delegate signing key is authorized by the user's root wallet so the app can sign events without exposing the root key.
  docs: https://docs.towns.com/build/delegate-key-signing
  id: delegate-key-signing
  type: delegated-key
- description: AuthenticationService.StartAuthentication / FinishAuthentication issue a short-lived session used to authorize Stream RPC (StreamService) calls.
  evidence: protocol/auth.proto AuthenticationService.
  id: rpc-session
  type: session-token
- description: Bots/apps receive an APP_PRIVATE_DATA credential (private key + encryption device) at registration time, used to sign and decrypt on behalf of the app.
  evidence: docs bots getting-started; apps.proto AppRegistryService.Register / RotateSecret.
  id: app-identity
  type: app-credential
- description: Inbound webhook requests from Towns servers to a bot are verified using the bot's JWT_SECRET issued at creation.
  evidence: docs bots getting-started.
  id: webhook-jwt
  type: jwt
slug: here-not-there-labs-authentication
source_filename: here-not-there-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  docs.towns.com (bots getting-started, delegate-key-signing, react-sdk),\n  protocol/auth.proto (AuthenticationService), and the first-party siwe package.\n  No REST OpenAPI securitySchemes are published (the docs OpenAPI endpoint serves\n  a Mintlify sample), so this profile is derived from the SDK/bot docs and proto.\nprovider: Here Not There Labs\nproduct: Towns Protocol\ndocs: https://docs.towns.com/build/bots/getting-started\nsummary: >-\n  Towns is a wallet-native, decentralized protocol. End users authenticate by\n  signing with an Ethereum wallet (Sign-In with Ethereum / EIP-4361 via the\n  first-party siwe library), typically using a delegate key so the root wallet\n  key is not exposed. Bots/apps authenticate with a protocol-issued app identity\n  (APP_PRIVATE_DATA) and verify inbound webhooks with a JWT_SECRET. At the RPC\n  layer, AuthenticationService issues a short-lived session for Stream RPC calls.\nschemes:\n\
  - id: siwe\n  type: wallet-signature\n  standard: EIP-4361 (Sign-In with Ethereum)\n  description: >-\n    Users sign a SIWE message with their Ethereum wallet to establish identity.\n    Implemented via the first-party @towns-protocol siwe library.\n  evidence: siwe package published by the org; connectTowns / signAndConnect react hooks.\n- id: delegate-key-signing\n  type: delegated-key\n  description: >-\n    A delegate signing key is authorized by the user's root wallet so the app can\n    sign events without exposing the root key.\n  docs: https://docs.towns.com/build/delegate-key-signing\n- id: rpc-session\n  type: session-token\n  description: >-\n    AuthenticationService.StartAuthentication / FinishAuthentication issue a\n    short-lived session used to authorize Stream RPC (StreamService) calls.\n  evidence: protocol/auth.proto AuthenticationService.\n- id: app-identity\n  type: app-credential\n  description: >-\n    Bots/apps receive an APP_PRIVATE_DATA credential (private key\
  \ + encryption\n    device) at registration time, used to sign and decrypt on behalf of the app.\n  evidence: docs bots getting-started; apps.proto AppRegistryService.Register / RotateSecret.\n- id: webhook-jwt\n  type: jwt\n  description: >-\n    Inbound webhook requests from Towns servers to a bot are verified using the\n    bot's JWT_SECRET issued at creation.\n  evidence: docs bots getting-started.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/here-not-there-labs/refs/heads/main/authentication/here-not-there-labs-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Messaging
- Decentralized
- Web3
- Blockchain
- Protocol
- Chat
- Bots
- Encryption
- SDK
---
