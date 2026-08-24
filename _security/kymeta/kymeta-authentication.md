---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Kymeta Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
- refreshToken
overview: Kymeta secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, deviceCode, and refreshToken flow(s).
provider_name: Kymeta
provider_slug: kymeta
scheme_count: 2
schemes:
- dynamic_client_registration: false
  endpoints:
    authorization: https://access.kymeta.io/connect/authorize
    device_authorization: https://access.kymeta.io/connect/deviceauthorization
    end_session: https://access.kymeta.io/connect/endsession
    introspection: https://access.kymeta.io/connect/introspect
    jwks: https://access.kymeta.io/.well-known/openid-configuration/jwks
    revocation: https://access.kymeta.io/connect/revocation
    token: https://access.kymeta.io/connect/token
    userinfo: https://access.kymeta.io/connect/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  issuer: https://access.kymeta.io
  name: KymetaAccessOIDC
  openIdConnectUrl: https://access.kymeta.io/.well-known/openid-configuration
  operator: kymeta
  pkce_methods:
  - plain
  - S256
  response_types:
  - code
  - token
  - id_token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  scope_count: 11
  scopes_ref: scopes/kymeta-scopes.yml
  sources:
  - well-known/kymeta-access-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- dynamic_client_registration: true
  endpoints:
    authorization: https://academy.kymeta.io/api/v6/idam/oauth/authorize
    jwks: https://academy.kymeta.io/.well-known/jwks
    registration: https://academy.kymeta.io/api/v6/idam/oauth/clients/register
    revocation: https://academy.kymeta.io/api/v6/idam/oauth/token/revoke
    token: https://academy.kymeta.io/api/v6/idam/oauth/token
    userinfo: https://academy.kymeta.io/api/v6/idam/oauth/userinfo
  grant_types:
  - authorization_code
  - refresh_token
  id_token_signing_alg:
  - RS256
  issuer: https://academy.kymeta.io/
  name: KymetaAcademyOIDC
  openIdConnectUrl: https://academy.kymeta.io/.well-known/openid-configuration
  operator: vendor
  operator_note: Absorb LMS running on a Kymeta hostname. Endpoints are /api/v6/idam/oauth/*, scopes are absorb:learner and absorb:admin. Recorded because Kymeta's domain serves it, not because the API is Kymeta's.
  pkce_methods:
  - S256
  sources:
  - well-known/kymeta-academy-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  type: openIdConnect
slug: kymeta-authentication
source_filename: kymeta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://access.kymeta.io/.well-known/openid-configuration\nnote: >-\n  Derived entirely from documents Kymeta itself serves. Kymeta publishes no OpenAPI, so this\n  profile is built from the live OpenID Connect discovery document at its own identity provider\n  rather than from securitySchemes. derive-authentication.py was not run because there is no\n  spec in openapi/ for it to read.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, deviceCode, refreshToken]\n  machine_to_machine: true\n  machine_to_machine_evidence: >-\n    client_credentials is listed in grant_types_supported, so Kymeta issues non-interactive\n    tokens — the prerequisite for any partner or agent integration against api.kymeta.io.\nschemes:\n  - name: KymetaAccessOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://access.kymeta.io/.well-known/openid-configuration\n   \
  \ issuer: https://access.kymeta.io\n    operator: kymeta\n    sources: [well-known/kymeta-access-openid-configuration.json]\n    endpoints:\n      authorization: https://access.kymeta.io/connect/authorize\n      token: https://access.kymeta.io/connect/token\n      userinfo: https://access.kymeta.io/connect/userinfo\n      introspection: https://access.kymeta.io/connect/introspect\n      revocation: https://access.kymeta.io/connect/revocation\n      device_authorization: https://access.kymeta.io/connect/deviceauthorization\n      end_session: https://access.kymeta.io/connect/endsession\n      jwks: https://access.kymeta.io/.well-known/openid-configuration/jwks\n    grant_types: [authorization_code, client_credentials, refresh_token, implicit, 'urn:ietf:params:oauth:grant-type:device_code']\n    response_types: [code, token, id_token, 'id_token token', 'code id_token', 'code token', 'code id_token token']\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    id_token_signing_alg:\
  \ [RS256]\n    pkce_methods: [plain, S256]\n    scope_count: 11\n    scopes_ref: scopes/kymeta-scopes.yml\n    dynamic_client_registration: false\n  - name: KymetaAcademyOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://academy.kymeta.io/.well-known/openid-configuration\n    issuer: https://academy.kymeta.io/\n    operator: vendor\n    operator_note: >-\n      Absorb LMS running on a Kymeta hostname. Endpoints are /api/v6/idam/oauth/*, scopes are\n      absorb:learner and absorb:admin. Recorded because Kymeta's domain serves it, not because\n      the API is Kymeta's.\n    sources: [well-known/kymeta-academy-openid-configuration.json]\n    endpoints:\n      authorization: https://academy.kymeta.io/api/v6/idam/oauth/authorize\n      token: https://academy.kymeta.io/api/v6/idam/oauth/token\n      userinfo: https://academy.kymeta.io/api/v6/idam/oauth/userinfo\n      revocation: https://academy.kymeta.io/api/v6/idam/oauth/token/revoke\n      registration: https://academy.kymeta.io/api/v6/idam/oauth/clients/register\n\
  \      jwks: https://academy.kymeta.io/.well-known/jwks\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, private_key_jwt, client_secret_basic]\n    id_token_signing_alg: [RS256]\n    pkce_methods: [S256]\n    dynamic_client_registration: true\ngaps:\n  - >-\n    No public authentication guide. Kymeta documents no getting-started, key-issuance or token\n    flow anywhere a member of the public can reach; the discovery document is the only published\n    description of how to authenticate.\n  - >-\n    api.kymeta.io serves no /.well-known/oauth-protected-resource, so an agent cannot discover\n    from the resource server which authorization server protects it (RFC 9728).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kymeta/refs/heads/main/authentication/kymeta-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Satellite
- Satellite Communications
- Connectivity
- Telecommunications
- Networking
- Antennas
- Metamaterials
- Aerospace and Defense
- Maritime
- Remote Monitoring
- Hardware
---
