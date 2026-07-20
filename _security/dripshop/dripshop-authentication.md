---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Dripshop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dripshop secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dripshop
provider_slug: dripshop
scheme_count: 1
schemes:
- bearer_format: JWT
  description: App-issued bearer token required by nearly all queries and mutations. Presented on the Authorization header. Minted by the login mutations below.
  name: bearerAuth
  scheme: bearer
  sources:
  - graphql/dripshop-schema.graphql
  type: http
slug: dripshop-authentication
source_filename: dripshop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: >-\n  graphql/dripshop-schema.graphql + live behavior probe of\n  https://api.dripshop.live/graphql\nnotes: >-\n  Derived from the GraphQL schema and observed endpoint behavior; Drip Shop publishes no\n  developer auth documentation. The GraphQL introspection does not declare formal\n  securitySchemes (GraphQL has no equivalent), so the model below is inferred from the\n  operation surface and from probing: an unauthenticated `query { health }` succeeds while\n  `query { me { id } }` returns an errors[] payload, indicating per-operation\n  authentication with a bearer token on the Authorization header.\nsummary:\n  types:\n  - http\n  - oauth2\n  http_scheme: bearer\n  bearer_format: JWT\n  transport: Authorization header (Bearer token)\n  public_operations:\n  - health\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    App-issued bearer token required by nearly all queries\
  \ and mutations. Presented on the\n    Authorization header. Minted by the login mutations below.\n  sources:\n  - graphql/dripshop-schema.graphql\nlogin_flows:\n- name: Wallet / crypto sign-in\n  operations:\n  - connectOrLoginWithWallet\n  - requiresUserWalletApproval\n  - getUserWalletDelegatePermission\n  description: Web3 wallet-based authentication (Solana / Base / EVM), the crypto-native path.\n- name: Farcaster\n  operations:\n  - createFarcasterUser\n  - farcasterUser\n  description: Farcaster identity used by the Drip Farcaster mini-app.\n- name: Facebook OAuth\n  operations:\n  - facebookOAuthUrl\n  - facebookOAuthSdkLogin\n  - facebookOAuthDesiredScopes\n  description: Facebook login and Graph API linking for simulcast to Facebook Live / Groups.\n- name: Twitch OAuth\n  operations:\n  - createTwitchUser\n  - twitchUser\n  description: Twitch account linking for simulcasting.\n- name: YouTube OAuth\n  operations:\n  - createYoutubeUser\n  - refreshYoutubeUser\n  - youtubeUser\n\
  \  description: YouTube account linking for simulcasting.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dripshop/refs/heads/main/authentication/dripshop-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- Live Shopping
- Collectibles
- Trading Cards
- Marketplace
- Ecommerce
- Auctions
- Live Streaming
- Payments
- GraphQL
---
