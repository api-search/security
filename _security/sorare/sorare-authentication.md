---
api_key_in:
- header
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sorare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Sorare secures its APIs with http, oauth2, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Sorare
provider_slug: sorare
scheme_count: 3
schemes:
- bearer_format: JWT
  description: 'JWT obtained from the GraphQL `signIn` mutation. The client first fetches the per-user bcrypt salt via GET https://api.sorare.com/api/v1/users/<email>, hashes the password client-side, then calls `signIn` with a mandatory `aud` audience identifier. Tokens are valid for 30 days and are sent as `Authorization: Bearer <token>` together with a `JWT-AUD: <aud>` header.'
  name: jwtBearer
  scheme: bearer
  token_lifetime: 30 days
  two_factor:
    flow: When 2FA is enabled, `signIn` returns an `otpSessionChallenge`; a second `signIn` call supplies `otpSessionChallenge` plus a one-time `otpAttempt` code.
    mechanism: totp
    supported: true
  type: http
- description: OAuth 2.0 for third-party apps acting on behalf of a Sorare user. Client ID and secret are requested through the Sorare Help Center; a callback URL must be registered. Access tokens are valid for 2 hours and are issued with a refresh token.
  flows:
  - access_token_lifetime: 2 hours
    authorizationUrl: https://api.sorare.com/oauth/authorize
    flow: authorizationCode
    refresh: true
    tokenUrl: https://api.sorare.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.sorare.com/oauth/token
  name: oauth2
  revocation_endpoint: https://api.sorare.com/oauth/revoke
  type: oauth2
- description: Optional API key requested on demand for elevated rate limits (600 calls/minute vs 60 for a standard authenticated caller). Sent as the `APIKEY` header.
  in: header
  name: apiKey
  parameter_name: APIKEY
  type: apiKey
slug: sorare-authentication
source_filename: sorare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/sorare/api\ndocs: https://github.com/sorare/api#authentication\napi: GraphQL (https://api.sorare.com/graphql)\nsummary:\n  types: [http, oauth2, apiKey]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  mfa: totp\nschemes:\n  - name: jwtBearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      JWT obtained from the GraphQL `signIn` mutation. The client first fetches the\n      per-user bcrypt salt via GET https://api.sorare.com/api/v1/users/<email>, hashes\n      the password client-side, then calls `signIn` with a mandatory `aud` audience\n      identifier. Tokens are valid for 30 days and are sent as\n      `Authorization: Bearer <token>` together with a `JWT-AUD: <aud>` header.\n    token_lifetime: 30 days\n    two_factor:\n      supported: true\n      mechanism: totp\n      flow: >-\n\
  \        When 2FA is enabled, `signIn` returns an `otpSessionChallenge`; a second\n        `signIn` call supplies `otpSessionChallenge` plus a one-time `otpAttempt` code.\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 for third-party apps acting on behalf of a Sorare user. Client ID and\n      secret are requested through the Sorare Help Center; a callback URL must be\n      registered. Access tokens are valid for 2 hours and are issued with a refresh token.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.sorare.com/oauth/authorize\n        tokenUrl: https://api.sorare.com/oauth/token\n        refresh: true\n        access_token_lifetime: 2 hours\n      - flow: clientCredentials\n        tokenUrl: https://api.sorare.com/oauth/token\n    revocation_endpoint: https://api.sorare.com/oauth/revoke\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name: APIKEY\n    description: >-\n      Optional API key requested\
  \ on demand for elevated rate limits (600 calls/minute\n      vs 60 for a standard authenticated caller). Sent as the `APIKEY` header.\nnotes:\n  - Blockchain actions (bids, offers) additionally require signing payloads with a\n    Starkware private key via the @sorare/crypto library — this is a signing step, not\n    an API authentication scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorare/refs/heads/main/authentication/sorare-authentication.yml
summary_line: http/oauth2/apiKey · 3 schemes
tags:
- Company
- Crypto
- GraphQL
- Fantasy Sports
- NFT
- Blockchain
- Gaming
- Sports
- Web3
---
