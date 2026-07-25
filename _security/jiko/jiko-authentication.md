---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Jiko Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Jiko secures its APIs with oauth2, openIdConnect, and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Jiko
provider_slug: jiko
scheme_count: 2
schemes:
- api: jiko:jiko-customer-api
  client_authentication: private_key_jwt
  description: OAuth 2.0 / OpenID Connect. Two flows are supported depending on use case; all clients authenticate with Private Key JWT (client_assertion) — no shared secrets. PKCE is required and DPoP is optional.
  extensions:
    dpop: optional
    pkce: required
  flows:
  - authorizationUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/authorize
    flow: authorizationCode
    par_endpoint: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/par
    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token
    use_case: User-facing apps acting on behalf of users (self-service client setup via the Settings page).
  - flow: clientCredentials
    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token
    use_case: Machine-to-machine backend services (client setup via Jiko support).
  issuer: https://authentication-portal.sandbox-api.jikoservices.com
  jwks_uri: https://authentication-portal.sandbox-api.jikoservices.com/.well-known/jwks.json
  name: CustomerOAuth2
  token_endpoint_auth_signing_alg:
  - PS256
  - EdDSA
  token_lifetimes:
    access_token: 15 minutes
    refresh_token: 90 days (authorization code flow only)
  type: oauth2
  userinfo_endpoint: https://authentication-portal.sandbox-api.jikoservices.com/api/v1/user
- api: jiko:jiko-partner-api
  description: Partners receive a username, password and shared secret from Jiko, and obtain a bearer token from the Login endpoint (POST /api/v1/login/). The token is sent in the Authorization header and has a 60-minute lifetime; the partner re-logs in when it expires.
  name: PartnerBearer
  network: Requests must originate from an IP address allowlisted by Jiko.
  request_requirements:
  - header: Authorization
    value: Bearer <access_token>
  - header: x-jiko-idempotency
    value: random UUID unique per action (replay window 1 hour)
  - header: x-jiko-signature
    value: base64(HMAC-SHA256(x-jiko-idempotency + request pathname + body, shared_secret))
  scheme: bearer
  token_lifetime: 60 minutes
  type: http
slug: jiko-authentication
source_filename: jiko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.jiko.io/products/customer-api/guides/oauth/getting-started\ndocs:\n- https://docs.jiko.io/products/customer-api/guides/oauth/getting-started\n- https://docs.jiko.io/products/partner-api/authentication\n- https://authentication-portal.sandbox-api.jikoservices.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: CustomerOAuth2\n  api: jiko:jiko-customer-api\n  type: oauth2\n  description: OAuth 2.0 / OpenID Connect. Two flows are supported depending on use\n    case; all clients authenticate with Private Key JWT (client_assertion) — no shared\n    secrets. PKCE is required and DPoP is optional.\n  flows:\n  - flow: authorizationCode\n    use_case: User-facing apps acting on behalf of users (self-service client setup\n      via the Settings page).\n    authorizationUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/authorize\n\
  \    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token\n    par_endpoint: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/par\n  - flow: clientCredentials\n    use_case: Machine-to-machine backend services (client setup via Jiko support).\n    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token\n  client_authentication: private_key_jwt\n  token_endpoint_auth_signing_alg: [PS256, EdDSA]\n  extensions:\n    pkce: required\n    dpop: optional\n  token_lifetimes:\n    access_token: 15 minutes\n    refresh_token: 90 days (authorization code flow only)\n  issuer: https://authentication-portal.sandbox-api.jikoservices.com\n  jwks_uri: https://authentication-portal.sandbox-api.jikoservices.com/.well-known/jwks.json\n  userinfo_endpoint: https://authentication-portal.sandbox-api.jikoservices.com/api/v1/user\n- name: PartnerBearer\n  api: jiko:jiko-partner-api\n  type: http\n  scheme: bearer\n  description:\
  \ Partners receive a username, password and shared secret from Jiko, and\n    obtain a bearer token from the Login endpoint (POST /api/v1/login/). The token\n    is sent in the Authorization header and has a 60-minute lifetime; the partner\n    re-logs in when it expires.\n  token_lifetime: 60 minutes\n  request_requirements:\n  - header: Authorization\n    value: Bearer <access_token>\n  - header: x-jiko-idempotency\n    value: random UUID unique per action (replay window 1 hour)\n  - header: x-jiko-signature\n    value: base64(HMAC-SHA256(x-jiko-idempotency + request pathname + body, shared_secret))\n  network: Requests must originate from an IP address allowlisted by Jiko.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jiko/refs/heads/main/authentication/jiko-authentication.yml
summary_line: oauth2/openIdConnect/http · 2 schemes
tags:
- Company
- Banking
- Payments
- Treasury
- Embedded Finance
- Fintech
- Cards
- Settlement
- Broker-Dealer
- Banking as a Service
---
