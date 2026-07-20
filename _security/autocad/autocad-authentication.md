---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Autocad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: AutoCAD secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: AutoCAD
provider_slug: autocad
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    description: Three-legged (3LO) user-context authorization.
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://developer.api.autodesk.com/authentication/v2/token
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  - description: Two-legged (2LO) application-context authorization.
    flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  issuer: https://developer.api.autodesk.com
  name: OAuth2
  type: oauth2
- id_token_signing_alg:
  - RS256
  introspection_endpoint: https://developer.api.autodesk.com/authentication/v2/introspect
  jwks_uri: https://developer.api.autodesk.com/authentication/v2/keys
  name: OpenIDConnect
  openIdConnectUrl: https://developer.api.autodesk.com/.well-known/openid-configuration
  revocation_endpoint: https://developer.api.autodesk.com/authentication/v2/revoke
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://api.userprofile.autodesk.com/userinfo
slug: autocad-authentication
source_filename: autocad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://developer.api.autodesk.com/.well-known/openid-configuration\ndocs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/overview/\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  api_key_in: []\n  notes: >-\n    Autodesk Platform Services (APS) uses OAuth 2.0 exclusively. Two-legged (2LO,\n    client_credentials) is used for app-level access; three-legged (3LO,\n    authorization_code + PKCE) is used for user-context access. Secure Service\n    Accounts (SSA) provide server-to-server access on behalf of a service identity.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    issuer: https://developer.api.autodesk.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n        tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n        refreshUrl:\
  \ https://developer.api.autodesk.com/authentication/v2/token\n        pkce: S256\n        description: Three-legged (3LO) user-context authorization.\n      - flow: clientCredentials\n        tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n        description: Two-legged (2LO) application-context authorization.\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://developer.api.autodesk.com/.well-known/openid-configuration\n    userinfo_endpoint: https://api.userprofile.autodesk.com/userinfo\n    jwks_uri: https://developer.api.autodesk.com/authentication/v2/keys\n    revocation_endpoint: https://developer.api.autodesk.com/authentication/v2/revoke\n    introspection_endpoint: https://developer.api.autodesk.com/authentication/v2/introspect\n    id_token_signing_alg: [RS256]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\nendpoints:\n  authorize: https://developer.api.autodesk.com/authentication/v2/authorize\n\
  \  token: https://developer.api.autodesk.com/authentication/v2/token\n  keys: https://developer.api.autodesk.com/authentication/v2/keys\n  revoke: https://developer.api.autodesk.com/authentication/v2/revoke\n  introspect: https://developer.api.autodesk.com/authentication/v2/introspect\n  userinfo: https://api.userprofile.autodesk.com/userinfo\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocad/refs/heads/main/authentication/autocad-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- 3D Modeling
- Architecture
- CAD
- Design
- Drawing
- Engineering
---
