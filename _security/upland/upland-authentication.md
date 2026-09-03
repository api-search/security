---
api_key_in: []
api_specs:
- filename: upland-developers-api-openapi.json
  format: json
  label: Upland Developers API
  slug: upland-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-developers-api-openapi.json
- filename: upland-appchain-history-swagger.json
  format: json
  label: Upland Appchain History & Chain API
  slug: upland-appchain-history-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/openapi/upland-appchain-history-swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Upland Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upland secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Upland
provider_slug: upland
scheme_count: 2
schemes:
- applies_to: 'Every application-level operation: /auth/otp/init, all /containers*, /tracks, /buildings, /cities, /properties, /v2/properties, /neighborhoods, /collections, /treasures-history, /devshops*, /app-usage/webhook-calls, and all /rumble-tournament* operations except /rumble-tournaments/{id}/join.'
  credential_password: Application Secret Key (issued once, when the application is created)
  credential_username: Application ID (shown on the Developers Portal home screen)
  docs: https://docs.developers.upland.me/upland-developers/application-management/activating-an-application
  header: Authorization
  in: header
  name: basic
  rotation: The secret key cannot be retrieved after issue. To rotate, the developer must inactivate and then reactivate the application, which issues a new access token and has downstream impact on live integrations.
  scheme: basic
  source: openapi/upland-developers-api-openapi.json
  type: http
- applies_to: 'Player-scoped operations: GET /user/profile, GET /user/balances, GET /user/assets/nfts, GET /user/assets/properties, GET /user/travels, POST /user/join, and POST /rumble-tournaments/{id}/join.'
  bearer_format: JWT
  delivery: webhook
  docs: https://docs.developers.upland.me/upland-developers/api-definitions/upland-users-authentication
  header: Authorization
  in: header
  name: bearer
  scheme: bearer
  source: openapi/upland-developers-api-openapi.json
  type: http
slug: upland-authentication
source_filename: upland-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://docs.developers.upland.me/upland-developers/api-definitions/upland-users-authentication\ndocs:\n- https://docs.developers.upland.me/upland-developers/api-definitions/upland-users-authentication\n- https://docs.developers.upland.me/upland-developers/sign-up-and-authentication/1.-developers-sign-up\n- https://docs.developers.upland.me/upland-developers/application-management/third-party-applications\n- https://docs.developers.upland.me/upland-developers/api-definitions/api-information-production\nderived_from:\n- openapi/upland-developers-api-openapi.json\n- openapi/upland-developers-api-sandbox-openapi.json\nsummary:\n  types:\n  - http\n  models: 2\n  note: >-\n    Two distinct credentials, both declared in the OpenAPI securitySchemes and both documented.\n    Application identity is HTTP Basic (App ID as username, App Secret Key as password). Player\n    identity is an HTTP Bearer JWT that the application never requests\
  \ directly — it is PUSHED to\n    the application's registered webhook URL after the player pastes a connection code into their\n    Upland account. There is no OAuth 2.0 authorization server, no OIDC discovery document and no\n    scope endpoint anywhere on Upland's hosts (all /.well-known/* probes returned 404 or an SPA\n    shell), so no scopes/ artifact is emitted.\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  credential_username: Application ID (shown on the Developers Portal home screen)\n  credential_password: Application Secret Key (issued once, when the application is created)\n  applies_to: >-\n    Every application-level operation: /auth/otp/init, all /containers*, /tracks, /buildings,\n    /cities, /properties, /v2/properties, /neighborhoods, /collections, /treasures-history,\n    /devshops*, /app-usage/webhook-calls, and all /rumble-tournament* operations except\n    /rumble-tournaments/{id}/join.\n  rotation: >-\n    The\
  \ secret key cannot be retrieved after issue. To rotate, the developer must inactivate and\n    then reactivate the application, which issues a new access token and has downstream impact on\n    live integrations.\n  docs: https://docs.developers.upland.me/upland-developers/application-management/activating-an-application\n  source: openapi/upland-developers-api-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  applies_to: >-\n    Player-scoped operations: GET /user/profile, GET /user/balances, GET /user/assets/nfts,\n    GET /user/assets/properties, GET /user/travels, POST /user/join, and\n    POST /rumble-tournaments/{id}/join.\n  delivery: webhook\n  docs: https://docs.developers.upland.me/upland-developers/api-definitions/upland-users-authentication\n  source: openapi/upland-developers-api-openapi.json\nflows:\n- id: player-connection-code\n  name: Upland User connection code (OTP)\n  style: out-of-band one-time\
  \ code, token delivered by webhook\n  steps:\n  - Application calls POST /auth/otp/init with HTTP Basic (App ID + Secret Key). Operation id AuthController_otpInit.\n  - Upland returns a short connection code; the application displays, texts or emails it to the player.\n  - The player enters that code inside their own Upland account to grant the application access.\n  - >-\n      Upland POSTs an AuthenticationSuccess notification to the application's registered webhook URL\n      carrying code, userId (uuid) and accessToken (JWT). On failure or expiry it POSTs\n      AuthenticationFailure with code and message instead.\n  - The application uses that accessToken as an HTTP Bearer token on player-scoped operations.\n  revocation: >-\n    When a player disconnects the application from their Upland account, Upland POSTs a\n    UserDisconnectedApplication notification carrying appId and userId. The application is expected\n    to discard the player's token on that event.\n  docs: https://docs.developers.upland.me/upland-developers/api-definitions/upland-users-authentication\n\
  application_registration:\n  gate: approval\n  steps:\n  - Register a developer account and connect an Upland account; Upland runs a verification process taking up to 5 business days.\n  - Create an application supplying name, logo, description, container expiration time in hours, webhook URL, webhook access token and scope.\n  - Submit the application for review via the published ClickUp form; approval is required before production use.\n  - Register a Dev Shop (an owned Upland property with a qualifying construction) for production applications.\n  application_scopes:\n    note: >-\n      The application creation form exposes a fixed \"Scope\" field. Upland's documentation states the\n      only options are \"Read\" and \"Assets Transfer\". These are product-level application permissions\n      set in the Developers Portal, NOT OAuth scopes — they are not requested per token, not present\n      in the OpenAPI, and have no scope parameter on any operation.\n    values:\n    - Read\n \
  \   - Assets Transfer\n    source: https://docs.developers.upland.me/upland-developers/application-management/third-party-applications\n  docs: https://docs.developers.upland.me/upland-developers/application-management/submitting-an-application\nwebhook_authentication:\n  direction: Upland -> application\n  mechanism: >-\n    The developer supplies a Webhook URL and a Webhook Access Token when creating the application.\n    Upland presents that token on the notifications it POSTs, so the application can authenticate\n    inbound calls. Upland does not publish a signature scheme (no HMAC header is documented).\n  source: https://docs.developers.upland.me/upland-developers/application-management/third-party-applications\ndelegation:\n  name: Permission Delegation\n  status: alpha, opt-in by request\n  effect: >-\n    When enabled for a developer account, Upland can sign asset transfers on the developer's behalf,\n    removing the per-transaction manual signature. It enables the alternate\
  \ operation\n    POST /containers/{containerId}/join (EscrowController_putAssetsInEscrowContainerWithPermissionDelegation),\n    which takes App ID + Secret Key only and does not require the developer's EOS ID.\n  docs: https://docs.developers.upland.me/upland-developers/application-management/permission-delegation\ngaps:\n- No OAuth 2.0 or OpenID Connect. /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and /.well-known/openid-configuration all miss on every Upland host.\n- No published token lifetime, expiry or refresh mechanism for the player Bearer JWT.\n- No documented webhook signature (HMAC/JWS); inbound authenticity rests on a shared bearer token the developer chooses.\n- No mTLS, no API-key header scheme, no key-prefix convention.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upland/refs/heads/main/authentication/upland-authentication.yml
summary_line: http · 2 schemes
tags:
- Metaverse
- Web3
- Gaming
- Blockchain
- NFT
- Virtual Real Estate
- Digital Assets
- Escrow
- Tournaments
- Antelope
- Webhooks
- Developer Platform
---
