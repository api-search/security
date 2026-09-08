---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Adaptive Insurance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- tokenExchange
- implicit
- password
overview: Adaptive Insurance secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, tokenExchange, implicit, and password flow(s).
provider_name: Adaptive Insurance
provider_slug: adaptive-insurance
scheme_count: 1
schemes:
- endpoints:
    authorization: https://auth.adaptiveinsurance.com/authorize
    backchannel_authentication: https://auth.adaptiveinsurance.com/bc-authorize
    device_authorization: https://auth.adaptiveinsurance.com/oauth/device/code
    end_session: https://auth.adaptiveinsurance.com/oidc/logout
    jwks: https://auth.adaptiveinsurance.com/.well-known/jwks.json
    mfa_challenge: https://auth.adaptiveinsurance.com/mfa/challenge
    registration: https://auth.adaptiveinsurance.com/oidc/register
    revocation: https://auth.adaptiveinsurance.com/oauth/revoke
    token: https://auth.adaptiveinsurance.com/oauth/token
    userinfo: https://auth.adaptiveinsurance.com/userinfo
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.adaptiveinsurance.com/
  name: adaptive-auth0-tenant
  openIdConnectUrl: https://auth.adaptiveinsurance.com/.well-known/openid-configuration
  provider: Auth0 (custom domain)
  sources:
  - well-known/adaptive-insurance-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  - none
  type: openIdConnect
slug: adaptive-insurance-authentication
source_filename: adaptive-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://auth.adaptiveinsurance.com/.well-known/openid-configuration\nscope_note: >-\n  Adaptive Insurance publishes no public developer API and no API authentication guide.\n  What it DOES publish machine-readably is the OpenID Connect / RFC 8414 discovery\n  document for its own identity tenant at auth.adaptiveinsurance.com — an Auth0 custom\n  domain whose issuer is the company's own host. That tenant fronts the agent/broker\n  portal at app.adaptiveinsurance.com and the application backend at\n  api.adaptiveinsurance.com. This profile records that identity surface as probed; it is\n  NOT a published API authentication reference, and nothing here was derived from a\n  specification, because the company publishes none.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, deviceCode, tokenExchange, implicit, password]\n  pkce: true\n  pkce_methods:\
  \ [S256, plain]\n  mtls_bound_tokens: true\n  dpop: true\n  dpop_algs: [ES256]\n  mfa: true\n  dynamic_client_registration: true\nschemes:\n  - name: adaptive-auth0-tenant\n    type: openIdConnect\n    openIdConnectUrl: https://auth.adaptiveinsurance.com/.well-known/openid-configuration\n    issuer: https://auth.adaptiveinsurance.com/\n    provider: Auth0 (custom domain)\n    endpoints:\n      authorization: https://auth.adaptiveinsurance.com/authorize\n      token: https://auth.adaptiveinsurance.com/oauth/token\n      userinfo: https://auth.adaptiveinsurance.com/userinfo\n      jwks: https://auth.adaptiveinsurance.com/.well-known/jwks.json\n      revocation: https://auth.adaptiveinsurance.com/oauth/revoke\n      end_session: https://auth.adaptiveinsurance.com/oidc/logout\n      device_authorization: https://auth.adaptiveinsurance.com/oauth/device/code\n      backchannel_authentication: https://auth.adaptiveinsurance.com/bc-authorize\n      registration: https://auth.adaptiveinsurance.com/oidc/register\n\
  \      mfa_challenge: https://auth.adaptiveinsurance.com/mfa/challenge\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - tls_client_auth\n      - self_signed_tls_client_auth\n      - none\n    id_token_signing_algs: [HS256, RS256, PS256]\n    sources: ['well-known/adaptive-insurance-openid-configuration.json']\nconsumer_surfaces:\n  - surface: agent and broker portal\n    url: https://app.adaptiveinsurance.com/\n    signup: https://app.adaptiveinsurance.com/registration\n    auth: Auth0 universal login at https://auth.adaptiveinsurance.com/u/login\n  - surface: application backend\n    url: https://api.adaptiveinsurance.com/\n    note: >-\n      Live and reachable, answers with a JSON 404 envelope on every probed path. No\n      published specification, no /docs, no /openapi.json, no discovery document.\n      Treated as the portal's private backend, not a developer API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-insurance/refs/heads/main/authentication/adaptive-insurance-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Insurance
- Insurtech
- Parametric Insurance
- Specialty Insurance
- Climate Risk
- Weather Data
- Managing General Agent
- Flood
- Power Outage
---
