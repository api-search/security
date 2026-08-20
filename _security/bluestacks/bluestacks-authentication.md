---
api_key_in:
- header
api_specs:
- filename: bluestacks-payments-asyncapi.yml
  format: yaml
  label: now.gg Payments Server API
  slug: nowgg-payments-server-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluestacks/refs/heads/main/asyncapi/bluestacks-payments-asyncapi.yml
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bluestacks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Bluestacks secures its APIs with oauth2, http, and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Bluestacks
provider_slug: bluestacks
scheme_count: 5
schemes:
- api: now.gg User Account Service API
  credentials:
    client_id: issued per app in nowStudio under OAuth 2.0 Credentials
    client_secret: issued per app in nowStudio under OAuth 2.0 Credentials
    guidance: Docs explicitly warn against sharing one credential pair across apps, because revoking one app's access would interrupt all of them.
  flows:
  - flow: authorizationCode
    grant_type: code
    note: The authorization code is delivered to the app by the now.gg Login flow / account manager; no public authorization endpoint URL is documented in the API reference.
    tokenUrl: https://now.gg/accounts/oauth2/v1/token
  - flow: refreshToken
    grant_type: refresh_token
    tokenUrl: https://now.gg/accounts/oauth2/v1/token
  name: nowggOAuth2
  tokens:
  - claims:
    - iss
    - sub
    - aud
    - exp
    - iat
    - auth_time
    - email
    - mobile
    - userId
    - name
    - picture
    - countryCode
    format: JWT-shaped, verified via the verify-token endpoint
    issuer: https://now.gg
    name: id_token
    purpose: authentication — asserts who the player is
    used_by: basic login flow
  - claims:
    - iss
    - tokenId
    - aud
    - sessionId
    - userId
    - scope
    - iat
    - exp
    issuer: https://now.gg
    name: token
    purpose: authorization — bearer credential for the protected user APIs
    used_by: advanced (token-based) login integration flow
  - name: refresh_token
    purpose: mint a new `token` after expiry
  type: oauth2
  verification:
    body:
    - token_type
    - token
    - client_id
    - client_secret
    endpoint: POST https://now.gg/accounts/oauth2/v1/verify-token
    note: client_secret is required when token_type is `token`, optional when it is `id_token`. Verification is a provider-side call rather than local JWKS validation — no JWKS URI or OIDC discovery document is published.
- api: now.gg User Account Service API
  applies_to:
  - GET /accounts/users/v1/userinfo
  - GET /accounts/users/v1/sessioninfo
  header: 'Authorization: Bearer <token>'
  name: nowggBearer
  scheme: bearer
  type: http
- api: now.gg Payments Server API
  applies_to:
  - POST /v2/sellers/order/verifyPurchase
  - POST /v2/order/consumePurchase
  - POST /v2/seller/order/acknowledgepurchase
  errors:
  - code: 3900
    message: INVALID_AUTHORIZATION_KEY
  in: header
  name: paymentsApiKey
  name_in_request: Authorization
  note: The Payments API Key is sent as a RAW value in the Authorization header — no Bearer/Basic scheme prefix, contrary to RFC 7235. Issued in the nowStudio credentials section.
  type: apiKey
- api: now.gg Payments (v1, deprecated) and nowStudio CLI
  in: header
  name: publisherToken
  name_in_request: publisherToken
  note: Company-level credential copied from nowStudio > Account Information. Used by the deprecated v1 verifyPayment endpoint and by `nowgg init` in the CLI.
  type: apiKey
- direction: inbound-to-publisher
  in: header
  name: webhookApiKey
  name_in_request: Authorization
  note: Reversed direction — now.gg presents this key to the publisher's own SubscriptionStatusCallback / PaymentsProcessingCallback endpoint so the publisher can authenticate the caller. Generated and regenerated in nowStudio.
  type: apiKey
slug: bluestacks-authentication
source_filename: bluestacks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://docs.now.gg/user-account-service/api-reference\ndocs:\n- https://docs.now.gg/user-account-service/api-reference\n- https://docs.now.gg/user-account-service/authenticate-with-a-backend-server\n- https://docs.now.gg/payments/references/verifypurchase\n- https://docs.now.gg/nowstudio/start-using-nowstudio\nnote: >-\n  Derived by reading the published docs, not from an OpenAPI — now.gg publishes no\n  machine-readable specification for any of these surfaces. Four distinct credentials\n  are in play and they are not interchangeable: an OAuth 2.0 client_id/client_secret\n  pair for player login, a Payments API Key for the server-side purchase APIs, a\n  Publisher Token for nowStudio/CLI operations, and a Webhook API Key that now.gg\n  presents to the publisher's own callback endpoint.\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n\
  \  openid_connect_discovery: false\n  mtls: false\nschemes:\n- name: nowggOAuth2\n  type: oauth2\n  api: now.gg User Account Service API\n  flows:\n  - flow: authorizationCode\n    tokenUrl: https://now.gg/accounts/oauth2/v1/token\n    grant_type: code\n    note: >-\n      The authorization code is delivered to the app by the now.gg Login flow / account\n      manager; no public authorization endpoint URL is documented in the API reference.\n  - flow: refreshToken\n    tokenUrl: https://now.gg/accounts/oauth2/v1/token\n    grant_type: refresh_token\n  credentials:\n    client_id: issued per app in nowStudio under OAuth 2.0 Credentials\n    client_secret: issued per app in nowStudio under OAuth 2.0 Credentials\n    guidance: >-\n      Docs explicitly warn against sharing one credential pair across apps, because\n      revoking one app's access would interrupt all of them.\n  tokens:\n  - name: id_token\n    purpose: authentication — asserts who the player is\n    format: JWT-shaped, verified\
  \ via the verify-token endpoint\n    claims:\n    - iss\n    - sub\n    - aud\n    - exp\n    - iat\n    - auth_time\n    - email\n    - mobile\n    - userId\n    - name\n    - picture\n    - countryCode\n    issuer: https://now.gg\n    used_by: basic login flow\n  - name: token\n    purpose: authorization — bearer credential for the protected user APIs\n    claims:\n    - iss\n    - tokenId\n    - aud\n    - sessionId\n    - userId\n    - scope\n    - iat\n    - exp\n    issuer: https://now.gg\n    used_by: advanced (token-based) login integration flow\n  - name: refresh_token\n    purpose: mint a new `token` after expiry\n  verification:\n    endpoint: POST https://now.gg/accounts/oauth2/v1/verify-token\n    body:\n    - token_type\n    - token\n    - client_id\n    - client_secret\n    note: >-\n      client_secret is required when token_type is `token`, optional when it is\n      `id_token`. Verification is a provider-side call rather than local JWKS\n      validation — no JWKS URI\
  \ or OIDC discovery document is published.\n- name: nowggBearer\n  type: http\n  scheme: bearer\n  api: now.gg User Account Service API\n  header: 'Authorization: Bearer <token>'\n  applies_to:\n  - GET /accounts/users/v1/userinfo\n  - GET /accounts/users/v1/sessioninfo\n- name: paymentsApiKey\n  type: apiKey\n  in: header\n  name_in_request: Authorization\n  api: now.gg Payments Server API\n  note: >-\n    The Payments API Key is sent as a RAW value in the Authorization header — no\n    Bearer/Basic scheme prefix, contrary to RFC 7235. Issued in the nowStudio\n    credentials section.\n  applies_to:\n  - POST /v2/sellers/order/verifyPurchase\n  - POST /v2/order/consumePurchase\n  - POST /v2/seller/order/acknowledgepurchase\n  errors:\n  - code: 3900\n    message: INVALID_AUTHORIZATION_KEY\n- name: publisherToken\n  type: apiKey\n  in: header\n  name_in_request: publisherToken\n  api: now.gg Payments (v1, deprecated) and nowStudio CLI\n  note: >-\n    Company-level credential copied from\
  \ nowStudio > Account Information. Used by the\n    deprecated v1 verifyPayment endpoint and by `nowgg init` in the CLI.\n- name: webhookApiKey\n  type: apiKey\n  in: header\n  name_in_request: Authorization\n  direction: inbound-to-publisher\n  note: >-\n    Reversed direction — now.gg presents this key to the publisher's own\n    SubscriptionStatusCallback / PaymentsProcessingCallback endpoint so the publisher\n    can authenticate the caller. Generated and regenerated in nowStudio.\ngaps:\n- No /.well-known/openid-configuration and no /.well-known/oauth-authorization-server\n  on any host, so neither OIDC nor RFC 8414 discovery is possible.\n- No published JWKS endpoint; token validation requires a round trip to now.gg.\n- No documented authorization endpoint URL, redirect_uri handling, PKCE or state\n  parameter in the API reference.\n- The Payments API Key is a bare header value with no scheme prefix and no documented\n  rotation policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluestacks/refs/heads/main/authentication/bluestacks-authentication.yml
summary_line: oauth2/http/apiKey · 5 schemes
tags:
- Company
- Gaming
- Cloud Gaming
- Android
- Mobile
- Payments
- In-App Purchases
- Subscription
- Developer Platform
- App Distribution
- Advertising
- Authentication
---
