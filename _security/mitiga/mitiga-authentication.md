---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: Mitiga publishes no public developer documentation, but its product API gateway (api.mitiga.cloud) serves an anonymous RFC 8414 authorization-server metadata document. This profile is derived entirely from that document and the OIDC discovery document on the identity host it points at. No OpenAPI securitySchemes were available to derive from.
kind: authentication
layout: security
method: probed
name: Mitiga Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- deviceCode
- tokenExchange
- refreshToken
overview: Mitiga secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, deviceCode, tokenExchange, and refreshToken flow(s).
provider_name: Mitiga
provider_slug: mitiga
scheme_count: 2
schemes:
- backchannel_logout: true
  code_challenge_methods:
  - S256
  - plain
  dpop_signing_algs:
  - ES256
  dynamic_client_registration: true
  endpoints:
    authorization: https://api.mitiga.cloud/oauth-2/authorize
    backchannel_authentication: https://auth.mitiga.cloud/bc-authorize
    device_authorization: https://auth.mitiga.cloud/oauth/device/code
    jwks: https://api.mitiga.cloud/.well-known/jwks.json
    mfa_challenge: https://auth.mitiga.cloud/mfa/challenge
    registration: https://api.mitiga.cloud/oauth-2/oidc/register
    revocation: https://auth.mitiga.cloud/oauth/revoke
    token: https://api.mitiga.cloud/oauth-2/token
    userinfo: https://api.mitiga.cloud/oauth-2/userinfo
  global_token_revocation: true
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://api.mitiga.cloud/
  name: oauth2
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/mitiga-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_algs:
  - RS256
  - RS384
  - PS256
  type: oauth2
- issuer: https://auth.mitiga.cloud/
  name: openIdConnect
  openIdConnectUrl: https://auth.mitiga.cloud/.well-known/openid-configuration
  sources:
  - well-known/mitiga-openid-configuration.json
  type: openIdConnect
slug: mitiga-authentication
source_filename: mitiga-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://api.mitiga.cloud/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Mitiga publishes no public developer documentation, but its product API gateway\n  (api.mitiga.cloud) serves an anonymous RFC 8414 authorization-server metadata document.\n  This profile is derived entirely from that document and the OIDC discovery document on\n  the identity host it points at. No OpenAPI securitySchemes were available to derive from.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode, deviceCode, tokenExchange, refreshToken]\n  identity_provider: Auth0 (EU tenant)\n  proof_of_possession: DPoP (ES256)\n  pkce: true\nschemes:\n- name: oauth2\n  type: oauth2\n  issuer: https://api.mitiga.cloud/\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n  endpoints:\n    authorization: https://api.mitiga.cloud/oauth-2/authorize\n    token: https://api.mitiga.cloud/oauth-2/token\n\
  \    userinfo: https://api.mitiga.cloud/oauth-2/userinfo\n    registration: https://api.mitiga.cloud/oauth-2/oidc/register\n    jwks: https://api.mitiga.cloud/.well-known/jwks.json\n    device_authorization: https://auth.mitiga.cloud/oauth/device/code\n    revocation: https://auth.mitiga.cloud/oauth/revoke\n    backchannel_authentication: https://auth.mitiga.cloud/bc-authorize\n    mfa_challenge: https://auth.mitiga.cloud/mfa/challenge\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  token_endpoint_auth_methods:\n  -\
  \ client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_algs: [RS256, RS384, PS256]\n  id_token_signing_algs: [HS256, RS256, PS256]\n  code_challenge_methods: [S256, plain]\n  response_types: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n  response_modes: [query, fragment, form_post]\n  dpop_signing_algs: [ES256]\n  dynamic_client_registration: true\n  backchannel_logout: true\n  global_token_revocation: true\n- name: openIdConnect\n  type: openIdConnect\n  issuer: https://auth.mitiga.cloud/\n  openIdConnectUrl: https://auth.mitiga.cloud/.well-known/openid-configuration\n  sources: [well-known/mitiga-openid-configuration.json]\nnotes:\n- >-\n  Machine-to-machine access is possible in principle — client_credentials is an advertised\n  grant type — but no public documentation describes how a customer obtains a client id\n  and secret, and no scope beyond the standard OIDC set is advertised anonymously.\n\
  - >-\n  The customer console at https://mitiga.cloud redirects to the Auth0 universal login on\n  auth.mitiga.cloud; every product route behind the Kong gateway returns\n  \"no Route matched with those values\" to an unauthenticated caller.\nx-evidence:\n- url: https://api.mitiga.cloud/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-04'\n- url: https://auth.mitiga.cloud/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitiga/refs/heads/main/authentication/mitiga-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Security
- Cloud Security
- SaaS Security
- Cloud Detection and Response
- Incident Response
- Threat Detection
- Identity Security
- Managed Security Services
- Artificial Intelligence
---
