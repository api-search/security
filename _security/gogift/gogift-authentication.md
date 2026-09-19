---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'GoGift authenticates every API request with an OpenID Connect access token (a signed JWT) issued by its own IdentityServer-style authorization server. Integrators are issued a client id and client secret by GoGift, exchange them at the token endpoint, and send the resulting token as an HTTP Bearer credential on every call to api.gogift.io. There is no API-key mode and no anonymous surface: the docs state plainly that this is an HTTPS-only API with OpenID authentication and CORS support.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Gogift Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoGift declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: GoGift
provider_slug: gogift
scheme_count: 3
schemes:
- description: Production OpenID Connect discovery document. Issuer https://auth.gogift.io, RS256 id tokens, JWKS at https://auth.gogift.io/.well-known/openid-configuration/jwks.
  environment: production
  id: gogift_oidc
  openIdConnectUrl: https://auth.gogift.io/.well-known/openid-configuration
  type: openIdConnect
- description: Sandbox OpenID Connect discovery document. Issuer https://auth-pre.gogift.io.
  environment: sandbox
  id: gogift_oidc_sandbox
  openIdConnectUrl: https://auth-pre.gogift.io/.well-known/openid-configuration
  type: openIdConnect
- applies_to:
  - https://api.gogift.io
  - https://api-pre.gogift.io
  bearerFormat: JWT
  description: 'The access token returned by the token endpoint is presented to api.gogift.io as `Authorization: Bearer <jwt>`. The docs show this header on every documented endpoint.'
  id: gogift_bearer
  scheme: bearer
  type: http
slug: gogift-authentication
source_filename: gogift-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.gogift.io/#authentication
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://docs.gogift.io/#authentication\nsources:\n  - https://docs.gogift.io/#authentication\n  - https://docs.gogift.io/#authentication-example\n  - https://auth.gogift.io/.well-known/openid-configuration\n  - well-known/gogift-openid-configuration.json\nprovider: GoGift\nproviderId: gogift\ndescription: >-\n  GoGift authenticates every API request with an OpenID Connect access token (a signed JWT)\n  issued by its own IdentityServer-style authorization server. Integrators are issued a client\n  id and client secret by GoGift, exchange them at the token endpoint, and send the resulting\n  token as an HTTP Bearer credential on every call to api.gogift.io. There is no API-key mode\n  and no anonymous surface: the docs state plainly that this is an HTTPS-only API with OpenID\n  authentication and CORS support.\ndocs: https://docs.gogift.io/#authentication\nschemes:\n  - id: gogift_oidc\n    type: openIdConnect\n    openIdConnectUrl:\
  \ https://auth.gogift.io/.well-known/openid-configuration\n    description: >-\n      Production OpenID Connect discovery document. Issuer https://auth.gogift.io, RS256 id\n      tokens, JWKS at https://auth.gogift.io/.well-known/openid-configuration/jwks.\n    environment: production\n  - id: gogift_oidc_sandbox\n    type: openIdConnect\n    openIdConnectUrl: https://auth-pre.gogift.io/.well-known/openid-configuration\n    description: Sandbox OpenID Connect discovery document. Issuer https://auth-pre.gogift.io.\n    environment: sandbox\n  - id: gogift_bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      The access token returned by the token endpoint is presented to api.gogift.io as\n      `Authorization: Bearer <jwt>`. The docs show this header on every documented endpoint.\n    applies_to:\n      - https://api.gogift.io\n      - https://api-pre.gogift.io\ncredentials:\n  issued_by: GoGift (client id + client secret are provisioned by GoGift,\
  \ not self-service)\n  self_service: false\n  note: >-\n    The docs instruct integrators never to share the client secret when contacting GoGift\n    support; a department ID is the identifier GoGift asks for instead.\nflows:\n  - grant_type: client_credentials\n    supported: true\n    primary: true\n    token_endpoint: https://auth.gogift.io/connect/token\n    description: >-\n      Machine-to-machine flow used by server-side integrations. This is the flow the\n      published C#, PHP, Java and Node.js authentication examples demonstrate.\n  - grant_type: authorization_code\n    supported: true\n    authorization_endpoint: https://auth.gogift.io/connect/authorize\n    pkce: true\n    pkce_methods:\n      - S256\n      - plain\n  - grant_type: refresh_token\n    supported: true\n    note: Requires the `offline_access` scope.\n  - grant_type: urn:ietf:params:oauth:grant-type:device_code\n    supported: true\n    device_authorization_endpoint: https://auth.gogift.io/connect/deviceauthorization\n\
  \  - grant_type: password\n    supported: true\n    note: Advertised in the discovery document; legacy ROPC grant, not documented for API integrators.\n  - grant_type: implicit\n    supported: true\n    note: Advertised in the discovery document; legacy browser grant.\nendpoints:\n  issuer: https://auth.gogift.io\n  token: https://auth.gogift.io/connect/token\n  authorization: https://auth.gogift.io/connect/authorize\n  userinfo: https://auth.gogift.io/connect/userinfo\n  jwks: https://auth.gogift.io/.well-known/openid-configuration/jwks\n  introspection: https://auth.gogift.io/connect/introspect\n  revocation: https://auth.gogift.io/connect/revocation\n  end_session: https://auth.gogift.io/connect/endsession\ntoken:\n  format: JWT\n  signing_alg:\n    - RS256\n  transport: Authorization Bearer header\n  expires: true\n  expiry_documented: false\n  expiry_note: >-\n    The docs state \"The token has an expiration period so it cannot be used indefinitely\" and\n    tell integrators to implement\
  \ expiry/refresh handling, but do not publish the lifetime.\nclient_authentication:\n  - client_secret_basic\n  - client_secret_post\ntransport_security:\n  https_only: true\n  cors: true\n  source: https://docs.gogift.io/#overview\nwebhook_authentication:\n  mechanism: HMAC-SHA256 request signature\n  header: Signature\n  algorithm: hmac-sha256\n  style: HTTP Signatures (draft-cavage-http-signatures-07 style, keyId/algorithm/signature pairs)\n  secrets_required:\n    - ClientId\n    - WebhookSecret\n  note: >-\n    GoGift signs the outbound delivery-fulfilment webhook. The receiving endpoint validates\n    the `Signature` header using a ClientId and a WebhookSecret issued by GoGift. Reference\n    validation code is published in the docs under \"Webhook signature validation\".\n  source: https://docs.gogift.io/#information-about-webhook-delivery-fulfillment\nmtls: false\napi_keys: false\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gogift/refs/heads/main/authentication/gogift-authentication.yml
summary_line: 3 schemes
tags:
- Gift Cards
- Rewards
- Incentives
- Loyalty
- Commerce
- Payments
- Employee Recognition
---
