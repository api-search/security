---
api_key_in: []
api_specs:
- filename: line-messaging-api-openapi.yml
  format: yaml
  label: LINE Messaging API
  slug: line-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-messaging-api-openapi.yml
- filename: line-webhook-openapi.yml
  format: yaml
  label: LINE Messaging API Webhook
  slug: line-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-webhook-openapi.yml
- filename: line-channel-access-token-openapi.yml
  format: yaml
  label: LINE Channel Access Token API
  slug: line-channel-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-channel-access-token-openapi.yml
- filename: line-insight-openapi.yml
  format: yaml
  label: LINE Insight API
  slug: line-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-insight-openapi.yml
- filename: line-manage-audience-openapi.yml
  format: yaml
  label: LINE Manage Audience API
  slug: line-manage-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-manage-audience-openapi.yml
- filename: line-liff-openapi.yml
  format: yaml
  label: LIFF Server API
  slug: line-liff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-liff-openapi.yml
- filename: line-module-openapi.yml
  format: yaml
  label: LINE Module API
  slug: line-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-module-openapi.yml
- filename: line-module-attach-openapi.yml
  format: yaml
  label: LINE Module Attach API
  slug: line-module-attach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-module-attach-openapi.yml
- filename: line-shop-openapi.yml
  format: yaml
  label: LINE Mission Sticker API
  slug: line-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-shop-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Line Authentication
name_suffix: Authentication
oauth_flows: []
overview: LINE secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LINE
provider_slug: line
scheme_count: 3
schemes:
- applies_to:
  - openapi/line-messaging-api-openapi.yml
  - openapi/line-insight-openapi.yml
  - openapi/line-manage-audience-openapi.yml
  - openapi/line-liff-openapi.yml
  - openapi/line-module-openapi.yml
  - openapi/line-shop-openapi.yml
  bearerFormat: ChannelAccessToken
  description: Channel access token presented as an HTTP Bearer credential in the Authorization header. Scoped to a single LINE channel — rate limits and message quota are counted per channel, and endpoint entitlement is a property of the channel and the Official Account plan rather than of a scope claim.
  name: Bearer
  scheme: bearer
  token_types:
  - issued_by: LINE Developers Console
    name: long-lived channel access token
    note: Reissuing invalidates the previous token.
    ttl: no expiry until reissued
  - credentials: channel ID + channel secret (client_credentials style)
    endpoint: POST https://api.line.me/v2/oauth/accessToken
    name: short-lived channel access token (v2.0)
    operation: issueChannelToken
    revoke: revokeChannelToken (POST /v2/oauth/revoke)
    ttl: 30 days
    verify: verifyChannelToken (POST /v2/oauth/verify)
  - credentials: JWT assertion signed with an assertion signing key registered in the LINE Developers Console (RS256), exchanged via urn:ietf:params:oauth:grant-type:jwt-bearer.
    endpoint: POST https://api.line.me/oauth2/v2.1/token
    list: getsAllValidChannelAccessTokenKeyIds (GET /oauth2/v2.1/tokens/kid)
    name: channel access token v2.1 (JWT assertion)
    note: The only token type that supports issuing multiple valid tokens concurrently and rotating them without invalidating the others.
    operation: issueChannelTokenByJWT
    revoke: revokeChannelTokenByJWT (POST /oauth2/v2.1/revoke)
    ttl: configurable, up to 30 days
    verify: verifyChannelTokenByJWT (GET /oauth2/v2.1/verify)
  - credentials: client_credentials with channel ID + channel secret
    endpoint: POST https://api.line.me/oauth2/v3/token
    name: stateless channel access token (v3)
    operation: issueStatelessChannelToken
    rate_limit: 370 requests per second
    revoke: not revocable — expiry only
    ttl: 15 minutes
  type: http
- applies_to:
  - openapi/line-module-attach-openapi.yml
  description: HTTP Basic authentication used only by the Module Attach API on manager.line.biz — the module channel presents its channel ID and secret to attach a module channel to a LINE Official Account.
  host: https://manager.line.biz
  name: basicAuth
  scheme: basic
  type: http
- description: End-user authentication and authorization. Authorization code grant with optional PKCE (S256 only); ID tokens are ES256-signed JWTs verified against the JWKS at https://api.line.me/oauth2/v2.1/certs. Subject identifiers are pairwise, so a user ID is stable per channel and not portable across channels.
  endpoints:
    authorization: https://access.line.me/oauth2/v2.1/authorize
    jwks: https://api.line.me/oauth2/v2.1/certs
    revocation: https://api.line.me/oauth2/v2.1/revoke
    token: https://api.line.me/oauth2/v2.1/token
    userinfo: https://api.line.me/oauth2/v2.1/userinfo
  name: LINE Login (OAuth 2.0 / OpenID Connect)
  not_in_spec: This scheme is documented and machine-discoverable via OIDC discovery but is not represented in any of the nine published OpenAPI documents — the specs cover the bot/server surface only.
  openIdConnectUrl: https://access.line.me/.well-known/openid-configuration
  scopes:
  - openid
  - profile
  - email
  see: scopes/line-scopes.yml
  type: openIdConnect
slug: line-authentication
source_filename: line-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://developers.line.biz/en/docs/basics/channel-access-token/\nsource: >-\n  Derived from the securitySchemes of the nine OpenAPI documents harvested from\n  https://github.com/line/line-openapi, then upgraded from\n  https://developers.line.biz/en/docs/basics/channel-access-token/,\n  https://developers.line.biz/en/docs/line-login/integrate-line-login/ and the\n  OIDC discovery document at\n  https://access.line.me/.well-known/openid-configuration (probed 200).\nsummary:\n  types:\n    - http\n    - oauth2\n    - openIdConnect\n  primary: Bearer channel access token, scoped to a LINE channel\n  end_user_auth: LINE Login v2.1 (OAuth 2.0 authorization code + OpenID Connect)\nschemes:\n  - name: Bearer\n    type: http\n    scheme: bearer\n    bearerFormat: ChannelAccessToken\n    description: >-\n      Channel access token presented as an HTTP Bearer credential in the\n      Authorization header. Scoped to a single LINE channel\
  \ — rate limits and\n      message quota are counted per channel, and endpoint entitlement is a\n      property of the channel and the Official Account plan rather than of a\n      scope claim.\n    applies_to:\n      - openapi/line-messaging-api-openapi.yml\n      - openapi/line-insight-openapi.yml\n      - openapi/line-manage-audience-openapi.yml\n      - openapi/line-liff-openapi.yml\n      - openapi/line-module-openapi.yml\n      - openapi/line-shop-openapi.yml\n    token_types:\n      - name: long-lived channel access token\n        issued_by: LINE Developers Console\n        ttl: no expiry until reissued\n        note: Reissuing invalidates the previous token.\n      - name: short-lived channel access token (v2.0)\n        operation: issueChannelToken\n        endpoint: POST https://api.line.me/v2/oauth/accessToken\n        ttl: 30 days\n        credentials: channel ID + channel secret (client_credentials style)\n        verify: verifyChannelToken (POST /v2/oauth/verify)\n      \
  \  revoke: revokeChannelToken (POST /v2/oauth/revoke)\n      - name: channel access token v2.1 (JWT assertion)\n        operation: issueChannelTokenByJWT\n        endpoint: POST https://api.line.me/oauth2/v2.1/token\n        ttl: configurable, up to 30 days\n        credentials: >-\n          JWT assertion signed with an assertion signing key registered in the\n          LINE Developers Console (RS256), exchanged via\n          urn:ietf:params:oauth:grant-type:jwt-bearer.\n        verify: verifyChannelTokenByJWT (GET /oauth2/v2.1/verify)\n        revoke: revokeChannelTokenByJWT (POST /oauth2/v2.1/revoke)\n        list: getsAllValidChannelAccessTokenKeyIds (GET /oauth2/v2.1/tokens/kid)\n        note: >-\n          The only token type that supports issuing multiple valid tokens\n          concurrently and rotating them without invalidating the others.\n      - name: stateless channel access token (v3)\n        operation: issueStatelessChannelToken\n        endpoint: POST https://api.line.me/oauth2/v3/token\n\
  \        ttl: 15 minutes\n        credentials: client_credentials with channel ID + channel secret\n        revoke: not revocable — expiry only\n        rate_limit: 370 requests per second\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication used only by the Module Attach API on\n      manager.line.biz — the module channel presents its channel ID and secret\n      to attach a module channel to a LINE Official Account.\n    applies_to:\n      - openapi/line-module-attach-openapi.yml\n    host: https://manager.line.biz\n  - name: LINE Login (OAuth 2.0 / OpenID Connect)\n    type: openIdConnect\n    openIdConnectUrl: https://access.line.me/.well-known/openid-configuration\n    description: >-\n      End-user authentication and authorization. Authorization code grant with\n      optional PKCE (S256 only); ID tokens are ES256-signed JWTs verified\n      against the JWKS at https://api.line.me/oauth2/v2.1/certs. Subject\n      identifiers\
  \ are pairwise, so a user ID is stable per channel and not\n      portable across channels.\n    endpoints:\n      authorization: https://access.line.me/oauth2/v2.1/authorize\n      token: https://api.line.me/oauth2/v2.1/token\n      userinfo: https://api.line.me/oauth2/v2.1/userinfo\n      revocation: https://api.line.me/oauth2/v2.1/revoke\n      jwks: https://api.line.me/oauth2/v2.1/certs\n    scopes: [openid, profile, email]\n    not_in_spec: >-\n      This scheme is documented and machine-discoverable via OIDC discovery but\n      is not represented in any of the nine published OpenAPI documents — the\n      specs cover the bot/server surface only.\n    see: scopes/line-scopes.yml\ninbound_authentication:\n  webhook_signature:\n    header: x-line-signature\n    algorithm: Base64(HMAC-SHA256(channel secret, raw request body))\n    docs: https://developers.line.biz/en/docs/messaging-api/verify-webhook-signature/\n    note: >-\n      The bot server authenticates LINE, not the other way\
  \ round. Signature\n      must be computed over raw bytes before JSON parsing.\ngaps:\n  - >-\n    The published OpenAPI documents declare the Bearer scheme with only the\n    description \"Channel access token\" and no bearerFormat, so a generated\n    client cannot tell which of the four token flavours is expected.\n  - >-\n    No securityScheme at all is declared in channel-access-token.yml or\n    webhook.yml.\n  - >-\n    LINE Login is absent from the OpenAPI surface entirely; only OIDC discovery\n    describes it machine-readably.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/authentication/line-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Messaging
- Chatbots
- Social Login
- Mini Apps
- Marketing
- Webhook
- OpenID Connect
- Audience
- Analytics
- Japan
---
