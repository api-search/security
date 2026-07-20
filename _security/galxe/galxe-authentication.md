---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: Galxe exposes two distinct authentication surfaces. (1) The Integration / Server GraphQL API authenticates with a dashboard-issued API access token sent in the custom `access-token` request header. (2) "Sign in with Galxe" is a standard OAuth 2.0 authorization-code (with PKCE) identity flow that lets an app read a Galxe ID user's connected accounts and wallet addresses.
kind: authentication
layout: security
method: searched
name: Galxe Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Galxe secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Galxe
provider_slug: galxe
scheme_count: 2
schemes:
- description: 'Server API access token generated in the Galxe dashboard under Account → Settings → Server API → "Generate New API Tokens". Shown once; store securely. Sent as `access-token: <TOKEN>` on every GraphQL request to https://graphigo-business.prd.galaxy.eco/query.'
  errors:
  - code: TOKEN_REQUIRED
    http_status: 401
    meaning: access-token header missing
  - code: INVALID_TOKEN
    http_status: 401
    meaning: access-token invalid/revoked
  in: header
  name: accessToken
  obtain: https://dashboard.galxe.com/
  parameter_name: access-token
  type: apiKey
- authorizationUrl: https://app.galxe.com/oauth
  description: '"Sign in with Galxe" — OAuth 2.0 authorization-code grant (PKCE supported via code_challenge/code_challenge_method) granting access to a Galxe ID user''s connected identities. Authorization codes expire after 10 minutes; access tokens live 86400s (24h) with refresh-token support. Client IDs are issued on request via dashboard live-chat support.'
  docs: https://docs.galxe.com/galxe-id/galxe-id-integration/galxe-id-oauth
  flow: authorizationCode
  name: signInWithGalxe
  parameters:
  - client_id
  - client_secret
  - redirect_uri
  - state
  - code_challenge
  - code_challenge_method
  pkce: recommended
  tokenUrl: https://api.galxe.com/oauth/auth/2/token
  type: oauth2
slug: galxe-authentication
source_filename: galxe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.galxe.com/galxe-integration/getting-started/authentication\ndocs: https://docs.galxe.com/galxe-integration/getting-started/authentication\ndescription: >-\n  Galxe exposes two distinct authentication surfaces. (1) The Integration /\n  Server GraphQL API authenticates with a dashboard-issued API access token sent\n  in the custom `access-token` request header. (2) \"Sign in with Galxe\" is a\n  standard OAuth 2.0 authorization-code (with PKCE) identity flow that lets an\n  app read a Galxe ID user's connected accounts and wallet addresses.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: accessToken\n    type: apiKey\n    in: header\n    parameter_name: access-token\n    description: >-\n      Server API access token generated in the Galxe dashboard under Account →\n      Settings → Server API → \"Generate New API Tokens\". Shown once; store\n\
  \      securely. Sent as `access-token: <TOKEN>` on every GraphQL request to\n      https://graphigo-business.prd.galaxy.eco/query.\n    obtain: https://dashboard.galxe.com/\n    errors:\n      - code: TOKEN_REQUIRED\n        http_status: 401\n        meaning: access-token header missing\n      - code: INVALID_TOKEN\n        http_status: 401\n        meaning: access-token invalid/revoked\n  - name: signInWithGalxe\n    type: oauth2\n    flow: authorizationCode\n    pkce: recommended\n    authorizationUrl: https://app.galxe.com/oauth\n    tokenUrl: https://api.galxe.com/oauth/auth/2/token\n    docs: https://docs.galxe.com/galxe-id/galxe-id-integration/galxe-id-oauth\n    description: >-\n      \"Sign in with Galxe\" — OAuth 2.0 authorization-code grant (PKCE supported\n      via code_challenge/code_challenge_method) granting access to a Galxe ID\n      user's connected identities. Authorization codes expire after 10 minutes;\n      access tokens live 86400s (24h) with refresh-token support.\
  \ Client IDs are\n      issued on request via dashboard live-chat support.\n    parameters: [client_id, client_secret, redirect_uri, state, code_challenge, code_challenge_method]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galxe/refs/heads/main/authentication/galxe-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Crypto Web3
- Digital Identity
- Credentials
- Quests
- Loyalty
- GraphQL
- OAuth
- Blockchain
---
