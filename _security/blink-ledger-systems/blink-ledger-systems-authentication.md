---
api_key_in: []
api_specs:
- filename: blink-ledger-systems-authentication-api-openapi.yml
  format: yaml
  label: Blink Ledger Systems Authentication API
  slug: blink-ledger-systems-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blink-ledger-systems/refs/heads/main/openapi/blink-ledger-systems-authentication-api-openapi.yml
- filename: blink-ledger-systems-oauth-applications-api-openapi.yml
  format: yaml
  label: Blink Ledger Systems OAuth Applications API
  slug: blink-ledger-systems-oauth-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blink-ledger-systems/refs/heads/main/openapi/blink-ledger-systems-oauth-applications-api-openapi.yml
- filename: blink-ledger-systems-users-api-openapi.yml
  format: yaml
  label: Blink Ledger Systems Users API
  slug: blink-ledger-systems-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blink-ledger-systems/refs/heads/main/openapi/blink-ledger-systems-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Blink Ledger Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blink Ledger Systems declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Blink Ledger Systems
provider_slug: blink-ledger-systems
scheme_count: 6
schemes:
- description: Public merchant identifier passed as a query parameter when loading the Blink SDK. Also surfaced as merchant.alias in webhook payloads. Not a secret; identifies the publisher, does not authorize privileged calls.
  id: sdk_client_id
  in: query
  location: https://blink.net/1.0/blink-sdk.js?clientId=YOUR_CLIENT_ID
  name: clientId
  secret: false
  surface: browser-sdk
  type: apiKey
- description: Bearer token obtained by POSTing client-credential email/password to /users/login/. Required by /oauth/applications/register/, /oauth/applications/ and /oauth/access_token/.
  id: login_token
  in: header
  name: Authorization
  obtain:
    method: POST
    operation: getAuthToken
    path: /users/login/
    request:
      email: null
      password: null
    response:
      key: null
  scheme: bearer
  surface: server-side-api
  type: http
- description: Login with Blink. The browser SDK's getAuthorizationCode() opens a Blink login modal and returns an authorization code; the publisher's server exchanges that code plus client_id/client_secret at POST /oauth/access_token/ for the Blink user profile. grant_type accepts only "authorization_code". No scope parameter is documented — Blink publishes no scope registry, so no scopes/ artifact is emitted.
  flow: authorization_code
  id: oauth2_authorization_code
  registration_endpoint: /oauth/applications/register/
  scopes_documented: false
  surface: login-with-blink
  token_endpoint: /oauth/access_token/
  type: oauth2
- description: Optional shared secret chosen at webhook-registration time. Blink sends it as the Blink-Echo-Token request header on every notification POST so the receiver can verify origin.
  direction: inbound
  id: webhook_token
  in: header
  name: Blink-Echo-Token
  surface: webhooks
  type: apiKey
- algorithm: ed25519
  description: Every notification is signed over the canonical form of the `event` object (no whitespace, keys sorted lexicographically). The signature block carries algorithm, encoding, publicKey and signature so receivers that cannot store secrets can still verify authenticity.
  direction: inbound
  encoding: base16
  id: webhook_signature
  surface: webhooks
  type: signature
- algorithm: ed25519
  description: blinkSDK.requestPayment() accepts an optional merchantPublicKey and paymentInfoSignature proving the payment info (amount, currencyIsoCode, offerId, comment) was authorized by the merchant.
  direction: outbound
  encoding: base16
  id: payment_info_signature
  surface: browser-sdk
  type: signature
slug: blink-ledger-systems-authentication
source_filename: blink-ledger-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.blink.net/docs/server-side-api/api-overview.html\ndocs:\n  - https://docs.blink.net/docs/server-side-api/api-overview.html\n  - https://docs.blink.net/docs/server-side-api/get-auth-token.html\n  - https://docs.blink.net/docs/guides/login-with-blink.html\n  - https://docs.blink.net/docs/notifications/webHooks.html\nsummary: >-\n  Blink runs three distinct authentication surfaces: a public clientId that\n  scopes the browser SDK to a merchant, a bearer login token plus OAuth2\n  authorization-code exchange for the server-side API, and a dual\n  token/ed25519-signature scheme for inbound webhooks. Client credentials are\n  issued by Blink on request (integration@blink.net) — there is no\n  self-service key provisioning.\nschemes:\n  - id: sdk_client_id\n    type: apiKey\n    in: query\n    name: clientId\n    surface: browser-sdk\n    location: https://blink.net/1.0/blink-sdk.js?clientId=YOUR_CLIENT_ID\n    secret:\
  \ false\n    description: >-\n      Public merchant identifier passed as a query parameter when loading the\n      Blink SDK. Also surfaced as merchant.alias in webhook payloads. Not a\n      secret; identifies the publisher, does not authorize privileged calls.\n  - id: login_token\n    type: http\n    scheme: bearer\n    in: header\n    name: Authorization\n    surface: server-side-api\n    description: >-\n      Bearer token obtained by POSTing client-credential email/password to\n      /users/login/. Required by /oauth/applications/register/,\n      /oauth/applications/ and /oauth/access_token/.\n    obtain:\n      operation: getAuthToken\n      method: POST\n      path: /users/login/\n      request: {email, password}\n      response: {key}\n  - id: oauth2_authorization_code\n    type: oauth2\n    flow: authorization_code\n    surface: login-with-blink\n    description: >-\n      Login with Blink. The browser SDK's getAuthorizationCode() opens a Blink\n      login modal and returns\
  \ an authorization code; the publisher's server\n      exchanges that code plus client_id/client_secret at\n      POST /oauth/access_token/ for the Blink user profile. grant_type accepts\n      only \"authorization_code\". No scope parameter is documented — Blink\n      publishes no scope registry, so no scopes/ artifact is emitted.\n    token_endpoint: /oauth/access_token/\n    registration_endpoint: /oauth/applications/register/\n    scopes_documented: false\n  - id: webhook_token\n    type: apiKey\n    in: header\n    name: Blink-Echo-Token\n    surface: webhooks\n    direction: inbound\n    description: >-\n      Optional shared secret chosen at webhook-registration time. Blink sends it\n      as the Blink-Echo-Token request header on every notification POST so the\n      receiver can verify origin.\n  - id: webhook_signature\n    type: signature\n    algorithm: ed25519\n    encoding: base16\n    surface: webhooks\n    direction: inbound\n    description: >-\n      Every notification\
  \ is signed over the canonical form of the `event`\n      object (no whitespace, keys sorted lexicographically). The signature\n      block carries algorithm, encoding, publicKey and signature so receivers\n      that cannot store secrets can still verify authenticity.\n  - id: payment_info_signature\n    type: signature\n    algorithm: ed25519\n    encoding: base16\n    surface: browser-sdk\n    direction: outbound\n    description: >-\n      blinkSDK.requestPayment() accepts an optional merchantPublicKey and\n      paymentInfoSignature proving the payment info (amount, currencyIsoCode,\n      offerId, comment) was authorized by the merchant.\nprovisioning:\n  self_service: false\n  contact: integration@blink.net\n  note: >-\n    Client credentials, test-environment clientIds and webhook registrations\n    are all issued by Blink on request. Webhook registration goes through\n    biz.support@blink.net.\nenvironments:\n  production:\n    api_base: https://api.blink.net\n  test:\n    api_base:\
  \ https://api.test.blink.net\nrelated:\n  - errors/blink-ledger-systems-problem-types.yml\n  - conventions/blink-ledger-systems-conventions.yml\n  - openapi/blink-ledger-systems-server-side-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blink-ledger-systems/refs/heads/main/authentication/blink-ledger-systems-authentication.yml
summary_line: 6 schemes
tags:
- Company
- Infrastructure
- Payments
- Identity
- Authentication
- Publishing
- Media
- Subscription
- Donations
- Micropayments
- Paywall
- Webhook
---
