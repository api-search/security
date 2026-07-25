---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Marshmallow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- tokenExchange
overview: Marshmallow secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and tokenExchange flow(s).
provider_name: Marshmallow
provider_slug: marshmallow
scheme_count: 1
schemes:
- client_authentication:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  dpop:
    signing_algs:
    - RS256
    - RS384
    - RS512
    - PS256
    - PS384
    - PS512
    - ES256
    - ES384
    - ES512
    supported: true
  endpoints:
    authorization: https://auth.marshmallow.com/oauth2/authorize
    end_session: https://auth.marshmallow.com/connect/logout
    introspection: https://auth.marshmallow.com/oauth2/introspect
    jwks: https://auth.marshmallow.com/oauth2/jwks
    registration: null
    revocation: https://auth.marshmallow.com/oauth2/revoke
    token: https://auth.marshmallow.com/oauth2/token
    userinfo: https://auth.marshmallow.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_algs:
  - RS256
  issuer: https://auth.marshmallow.com
  mtls:
    certificate_bound_access_tokens: true
    client_authentication: true
  name: MarshmallowOpenIDConnect
  openIdConnectUrl: https://auth.marshmallow.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_types:
  - code
  scopes:
  - openid
  sources:
  - well-known/marshmallow-openid-configuration.json
  subject_types:
  - public
  type: openIdConnect
slug: marshmallow-authentication
source_filename: marshmallow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.marshmallow.com/.well-known/openid-configuration\nlocal_copy: well-known/marshmallow-openid-configuration.json\nnote: >-\n  Derived from the only machine-readable authentication artifact Marshmallow\n  publishes anonymously — its OpenID Connect discovery document. There is no\n  OpenAPI to derive securitySchemes from, and no public documentation of how a\n  third party obtains a client: registration is manual and partner-gated\n  (no dynamic client registration endpoint is advertised).\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, tokenExchange]\n  public_registration: false\n  self_serve: false\n  access: partner-gated\nschemes:\n- name: MarshmallowOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.marshmallow.com/.well-known/openid-configuration\n  issuer: https://auth.marshmallow.com\n  sources: [well-known/marshmallow-openid-configuration.json]\n\
  \  endpoints:\n    authorization: https://auth.marshmallow.com/oauth2/authorize\n    token: https://auth.marshmallow.com/oauth2/token\n    userinfo: https://auth.marshmallow.com/userinfo\n    jwks: https://auth.marshmallow.com/oauth2/jwks\n    revocation: https://auth.marshmallow.com/oauth2/revoke\n    introspection: https://auth.marshmallow.com/oauth2/introspect\n    end_session: https://auth.marshmallow.com/connect/logout\n    registration: null\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  response_types: [code]\n  client_authentication:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - self_signed_tls_client_auth\n  pkce:\n    supported: true\n    code_challenge_methods: [S256]\n  mtls:\n    client_authentication: true\n    certificate_bound_access_tokens: true\n  dpop:\n    supported: true\n    signing_algs: [RS256, RS384,\
  \ RS512, PS256, PS384, PS512, ES256, ES384, ES512]\n  id_token_signing_algs: [RS256]\n  subject_types: [public]\n  scopes: [openid]\nobservations:\n- >-\n  Sender-constrained tokens are supported two ways (mTLS certificate-bound per\n  RFC 8705 and DPoP per RFC 9449), which is the profile of an operator that\n  integrates with regulated financial counterparties rather than with the open\n  developer public.\n- >-\n  Token exchange (RFC 8693) is enabled, consistent with service-to-service\n  delegation inside Marshmallow's own estate and with named partners.\n- >-\n  Only the `openid` scope is advertised. No product scopes (quote, policy,\n  claim, payment) are published, so there is no anonymous way to reason about\n  what a partner client may do.\n- >-\n  No dynamic client registration (RFC 7591) endpoint is advertised; clients are\n  provisioned out of band.\ngaps:\n- No public documentation page describing the authentication flow.\n- No sandbox or test client credentials.\n- No published\
  \ product scopes or consent screens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marshmallow/refs/heads/main/authentication/marshmallow-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Insurance
- United Kingdom
- Insurtech
- Property and Casualty
- Motor Insurance
- Home Insurance
- Telematics
- Underwriting
- Claims
- Direct to Consumer
- Partner Gated
- No Public API
---
