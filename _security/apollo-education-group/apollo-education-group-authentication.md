---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Apollo Education Group Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- refreshToken
- deviceCode
- tokenExchange
- jwtBearer
- saml2Bearer
- ciba
- umaTicket
overview: Apollo Education Group secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, refreshToken, deviceCode, tokenExchange, jwtBearer, saml2Bearer, ciba, and umaTicket flow(s).
provider_name: Apollo Education Group
provider_slug: apollo-education-group
scheme_count: 1
schemes:
- endpoints:
    authorization: https://login.phoenix.edu:443/am/oauth2/authorize
    check_session_iframe: https://login.phoenix.edu:443/am/oauth2/connect/checkSession
    end_session: https://login.phoenix.edu:443/am/oauth2/connect/endSession
    introspection: https://login.phoenix.edu:443/am/oauth2/introspect
    jwks: https://login.phoenix.edu:443/am/oauth2/connect/jwk_uri
    pushed_authorization_request: https://login.phoenix.edu:443/am/oauth2/par
    registration: https://login.phoenix.edu:443/am/oauth2/register
    revocation: https://login.phoenix.edu:443/am/oauth2/token/revoke
    token: https://login.phoenix.edu:443/am/oauth2/access_token
    userinfo: https://login.phoenix.edu:443/am/oauth2/userinfo
  features:
    backchannel_logout: true
    backchannel_logout_session: true
    claims_parameter: false
    jarm_signed_authorization_response: true
    mtls_bound_access_tokens: true
    pushed_authorization_requests: supported (not required)
    request_object: supported (request and request_uri parameters both accepted)
  grant_types:
  - authorization_code
  - implicit
  - password
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:saml2-bearer
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - urn:openid:params:grant-type:ciba
  id_token_signing_algs:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - HS256
  - HS384
  - HS512
  issuer: https://login.phoenix.edu:443/am/oauth2
  name: PhoenixSSO
  openIdConnectUrl: https://login.phoenix.edu/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    note: '`plain` is still advertised alongside S256. RFC 7636 recommends S256 wherever the client can compute it; a server that keeps `plain` on the menu lets a weak client downgrade.'
    supported: true
  prompt_values:
  - none
  - login
  - consent
  response_modes:
  - query
  - fragment
  - form_post
  - jwt
  - query.jwt
  - fragment.jwt
  - form_post.jwt
  source: well-known/apollo-education-group-openid-configuration.json
  subject_types:
  - public
  - pairwise
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  - none
  type: openIdConnect
slug: apollo-education-group-authentication
source_filename: apollo-education-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://login.phoenix.edu/.well-known/openid-configuration\ndocs: null\nnote: |\n  Apollo Education Group / University of Phoenix publishes no developer API and therefore no\n  developer authentication documentation. The only authentication surface reachable without\n  credentials is the institution's own single sign-on: a ForgeRock Access Management OAuth 2.0 /\n  OpenID Connect authorization server on login.phoenix.edu, realm /alpha, which serves a public\n  OIDC discovery document anonymously (HTTP 200, 2026-09-04).\n\n  Everything below is read verbatim out of that discovery document. It is the authentication\n  profile for students, faculty and staff signing in to the MyPhoenix / eCampus portals — NOT a\n  third-party integration surface. Self-service developer registration does not exist: the\n  server advertises an RFC 7591 registration_endpoint, but ForgeRock exposes that path on every\n  deployment and it is not documented,\
  \ advertised, or reachable as a public onboarding route.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, password, refreshToken,\n    deviceCode, tokenExchange, jwtBearer, saml2Bearer, ciba, umaTicket]\n  self_service_signup: false\n  public_client_registration: false\n  mutual_tls: true\nsurfaces:\n  - name: University of Phoenix Single Sign-On (ForgeRock AM, realm /alpha)\n    base: https://login.phoenix.edu/am/oauth2\n    auth: oauth2 / openIdConnect\n    issuer: https://login.phoenix.edu:443/am/oauth2\n    evidence:\n      url: https://login.phoenix.edu/.well-known/openid-configuration\n      status: 200\n      probed: '2026-09-04'\n      content_type: application/json;charset=UTF-8\n    note: >-\n      Discovered by following https://portal.phoenix.edu/, which 302s into\n      /am/oauth2/authorize on this host with client_id f38408e4-9d02-4018-b109-000cdfc5982f and\n      redirect_uri https://sso.phoenix.edu/oidc/forgerock.\n\
  schemes:\n  - name: PhoenixSSO\n    type: openIdConnect\n    openIdConnectUrl: https://login.phoenix.edu/.well-known/openid-configuration\n    source: well-known/apollo-education-group-openid-configuration.json\n    issuer: https://login.phoenix.edu:443/am/oauth2\n    endpoints:\n      authorization: https://login.phoenix.edu:443/am/oauth2/authorize\n      token: https://login.phoenix.edu:443/am/oauth2/access_token\n      userinfo: https://login.phoenix.edu:443/am/oauth2/userinfo\n      jwks: https://login.phoenix.edu:443/am/oauth2/connect/jwk_uri\n      introspection: https://login.phoenix.edu:443/am/oauth2/introspect\n      revocation: https://login.phoenix.edu:443/am/oauth2/token/revoke\n      end_session: https://login.phoenix.edu:443/am/oauth2/connect/endSession\n      pushed_authorization_request: https://login.phoenix.edu:443/am/oauth2/par\n      registration: https://login.phoenix.edu:443/am/oauth2/register\n      check_session_iframe: https://login.phoenix.edu:443/am/oauth2/connect/checkSession\n\
  \    grant_types:\n      - authorization_code\n      - implicit\n      - password\n      - client_credentials\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:saml2-bearer\n      - urn:ietf:params:oauth:grant-type:uma-ticket\n      - urn:openid:params:grant-type:ciba\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt,\n      tls_client_auth, self_signed_tls_client_auth, none]\n    pkce:\n      supported: true\n      code_challenge_methods: [S256, plain]\n      note: >-\n        `plain` is still advertised alongside S256. RFC 7636 recommends S256 wherever the client\n        can compute it; a server that keeps `plain` on the menu lets a weak client downgrade.\n    id_token_signing_algs: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512,\n      HS256, HS384,\
  \ HS512]\n    subject_types: [public, pairwise]\n    response_modes: [query, fragment, form_post, jwt, query.jwt, fragment.jwt, form_post.jwt]\n    prompt_values: [none, login, consent]\n    features:\n      pushed_authorization_requests: supported (not required)\n      request_object: supported (request and request_uri parameters both accepted)\n      jarm_signed_authorization_response: true\n      mtls_bound_access_tokens: true\n      backchannel_logout: true\n      backchannel_logout_session: true\n      claims_parameter: false\nobservations:\n  - >-\n    The `password` (resource-owner credentials) and `implicit` grants are both still advertised.\n    OAuth 2.1 removes both; their presence on a 2026 deployment is a legacy-compatibility choice\n    worth noting, not a finding about a published developer product.\n  - >-\n    `require_pushed_authorization_requests` is false and `claims_parameter_supported` is false —\n    the server is a stock ForgeRock AM cloud deployment (version 3.0\
  \ discovery payload) rather\n    than a hardened FAPI profile.\n  - >-\n    No `oauth-protected-resource` (RFC 9728) document is served on this host (404), so there is\n    no protected-resource metadata for an agent to discover.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-education-group/refs/heads/main/authentication/apollo-education-group-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Education
- Higher Education
- Online Education
- Private Education
- University
---
