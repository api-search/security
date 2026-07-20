---
api_key_in: []
auth_types: []
description: LinQ does not use OAuth 2.0 or OpenID Connect. Access is granted by opaque bearer tokens minted by the LinQ auth services, seeded by a per-game secret key issued out of band at integration time. There are two access tokens and two auxiliary secrets.
kind: authentication
layout: security
method: searched
name: Linqgg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linq.gg declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Linq.gg
provider_slug: linqgg
scheme_count: 5
schemes:
- description: Minted for a game user from the game's private secret key plus the game's internal user id. Signs user transactions in conditional-anonymity mode.
  grants: anonymous-mode operations — balances, deposits, entry fees, tournament rewards
  id: access_token
  issued_by: AuthGameService.SignInGame
  kind: bearer
  lifetime: unlimited
  name: Access Token
  restrictions:
  - cannot transfer funds to the wallet account or other games
  - subject to a maximum stored-funds limit (anonymous total deposit limit 20.00)
  storage: persist on the user profile in the game backend
- description: Issued after the user authorizes through the LinQ app and links their game account to a real wallet account. Same header shape as Access Token, wider rights.
  grants: all operations including KYC, wallet transfer, withdrawal to bank or card
  id: wallet_token
  issued_by: AuthUserService.SignInGameUser
  kind: bearer
  lifetime: unlimited
  name: Wallet Token
  recommended_pattern: getAuthorization(user.walletToken ?? user.accessToken)
  storage: persist on the user profile; prefer over Access Token when both are held
- handling: Supply as an environment variable; docs recommend Google Secret Manager or equivalent. Must never be shipped in client code.
  id: private_secret_key
  issued: before integration begins, out of band
  kind: apiKey
  name: Private Secret Key
  usage: Server-to-server. Passed as the game_token field of SignInGameRequest to verify requests coming from the game backend and obtain a user Access Token.
- id: public_secret_key
  issued: before integration begins, out of band
  kind: apiKey
  name: Public Secret Key / Mobile SDK Secret Key
  usage: Initializes the LinQ Unity SDK and verifies requests originating from the front end. Set via LinqSDK.InitSDK(remoteUrl, secretKey) or the LinqSettings.asset editor config.
- description: Short-lived token handed to the LinQ app (via deep link or Keychain) to initiate account linking. Exchanged by SignInGameUser for a Wallet Token.
  id: secret_token
  issued_by: AuthUserService.SignUpGameUser
  kind: temporary
  lifetime: single use, for the linking handshake only
  name: Secret / User Token
slug: linqgg-authentication
source_filename: linqgg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.linq.gg/modules/auth/tokens\ndocs: https://docs.linq.gg/modules/auth\ndescription: >-\n  LinQ does not use OAuth 2.0 or OpenID Connect. Access is granted by opaque\n  bearer tokens minted by the LinQ auth services, seeded by a per-game secret\n  key issued out of band at integration time. There are two access tokens and\n  two auxiliary secrets.\ntransport:\n  protocol: grpc\n  header: authorization\n  format: 'Bearer <token>'\n  example_metadata: '{ meta: { authorization: `Bearer ${accessToken}` } }'\n  tls_required: true\nschemes:\n- id: access_token\n  kind: bearer\n  name: Access Token\n  issued_by: AuthGameService.SignInGame\n  description: >-\n    Minted for a game user from the game's private secret key plus the game's\n    internal user id. Signs user transactions in conditional-anonymity mode.\n  lifetime: unlimited\n  storage: persist on the user profile in the game backend\n  grants: anonymous-mode operations\
  \ — balances, deposits, entry fees, tournament rewards\n  restrictions:\n  - cannot transfer funds to the wallet account or other games\n  - subject to a maximum stored-funds limit (anonymous total deposit limit 20.00)\n- id: wallet_token\n  kind: bearer\n  name: Wallet Token\n  issued_by: AuthUserService.SignInGameUser\n  description: >-\n    Issued after the user authorizes through the LinQ app and links their game\n    account to a real wallet account. Same header shape as Access Token, wider\n    rights.\n  lifetime: unlimited\n  storage: persist on the user profile; prefer over Access Token when both are held\n  recommended_pattern: 'getAuthorization(user.walletToken ?? user.accessToken)'\n  grants: all operations including KYC, wallet transfer, withdrawal to bank or card\n- id: private_secret_key\n  kind: apiKey\n  name: Private Secret Key\n  usage: >-\n    Server-to-server. Passed as the game_token field of SignInGameRequest to\n    verify requests coming from the game backend and\
  \ obtain a user Access Token.\n  issued: before integration begins, out of band\n  handling: >-\n    Supply as an environment variable; docs recommend Google Secret Manager or\n    equivalent. Must never be shipped in client code.\n- id: public_secret_key\n  kind: apiKey\n  name: Public Secret Key / Mobile SDK Secret Key\n  usage: >-\n    Initializes the LinQ Unity SDK and verifies requests originating from the\n    front end. Set via LinqSDK.InitSDK(remoteUrl, secretKey) or the\n    LinqSettings.asset editor config.\n  issued: before integration begins, out of band\n- id: secret_token\n  kind: temporary\n  name: Secret / User Token\n  issued_by: AuthUserService.SignUpGameUser\n  description: >-\n    Short-lived token handed to the LinQ app (via deep link or Keychain) to\n    initiate account linking. Exchanged by SignInGameUser for a Wallet Token.\n  lifetime: single use, for the linking handshake only\nlinking_flows:\n- id: deep_link\n  description: >-\n    Game embeds the user_token\
  \ in a LinQ deep link. Falls back to the App Store\n    when the app is not installed.\n  schemes:\n    stage: 'linq-stg://?user_token={token}'\n    production: 'linq://?user_token={token}'\n  associated_domains:\n    stage: 'https://a.stg.linq.gg?user_token={token}'\n    production: 'https://a.linq.gg?user_token={token}'\n- id: keychain\n  description: >-\n    Apple-only fallback used when the LinQ app is not yet installed. The game\n    writes the token to a shared Keychain access group; the LinQ app reads it\n    after install and authorizes the game.\n  access_groups:\n    stage: $(AppIdentifierPrefix)games.galactica.linq.stg.shared\n    production: $(AppIdentifierPrefix)games.galactica.linq.shared\n  api: LinqUnity.Keychain.setAuthUserToken(token, accessGroup)\n  limitations:\n  - Apple ecosystem only; no Android equivalent published yet\n  - requires both apps to share one App Store account (game transferred to the\n    Galactica Games account)\n- id: sandbox_helper\n  description:\
  \ >-\n    HelpersService.VerifyPlayerToken emulates the user's in-app confirmation so\n    the linking handshake can be automated in integration tests. Test mode only.\nunauthenticated_operations:\n- linq.geo.restrictions.v2.RestrictionsService.IsAccessAllowed\nnotes:\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n  is published; there is no OAuth scope surface, so no scopes/ artifact exists.\n- Tokens carry no published expiry, so there is no documented refresh flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linqgg/refs/heads/main/authentication/linqgg-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Gaming
- Payments
- Wallet
- Loyalty
- Fintech
- Real Money Gaming
- gRPC
- Geolocation
- Authentication
---
