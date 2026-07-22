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
name: Sonrai Security Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- clientCredentials
overview: Sonrai Security secures its APIs with oauth2, openIdConnect, and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and clientCredentials flow(s).
provider_name: Sonrai Security
provider_slug: sonrai-security
scheme_count: 2
schemes:
- code_challenge_methods_supported:
  - S256
  - plain
  endpoints:
    authorization: https://login.sonraisecurity.com/authorize
    device_authorization: https://login.sonraisecurity.com/oauth/device/code
    jwks: https://login.sonraisecurity.com/.well-known/jwks.json
    revocation: https://login.sonraisecurity.com/oauth/revoke
    token: https://login.sonraisecurity.com/oauth/token
    userinfo: https://login.sonraisecurity.com/userinfo
  evidence: observed 302 to login.sonraisecurity.com/authorize with scope=openid+profile
  issuer: https://login.sonraisecurity.com/
  name: openIdConnect
  openIdConnectUrl: https://login.sonraisecurity.com/.well-known/openid-configuration
  provider: Auth0
  scopes_supported:
  - openid
  - profile
  - offline_access
  - email
  type: openIdConnect
- applies_to: Sonrai GraphQL API (https://app.sonraisecurity.com/graphql)
  evidence: CPF developer docs document a GraphQL API; the app.sonraisecurity.com/graphql endpoint responds (405 to unauthenticated probe) and the reference is gated behind the Auth0 login.
  name: bearerToken
  scheme: bearer
  type: http
slug: sonrai-security-authentication
source_filename: sonrai-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  Observed Auth0 OIDC authorize/login flow on login.sonraisecurity.com,\n  its /.well-known/openid-configuration, and the Sonrai CPF GraphQL API docs\n  (docs.sonraisecurity.com/cpf/api/sonrai-graphql-api). Detailed API-token docs\n  sit behind login in the gated /cpf developer section.\ndocs: https://docs.sonraisecurity.com/cpf/api/sonrai-graphql-api\nsummary:\n  types: [oauth2, openIdConnect, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, deviceCode, clientCredentials]\n  notes: >-\n    Interactive access to the Sonrai platform and its docs authenticates through\n    an Auth0-hosted OpenID Connect identity provider. The GraphQL API is called\n    with a bearer token over HTTPS. There is no unauthenticated public API\n    surface; the GraphQL endpoint requires an authenticated token.\nschemes:\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://login.sonraisecurity.com/.well-known/openid-configuration\n\
  \    issuer: https://login.sonraisecurity.com/\n    provider: Auth0\n    endpoints:\n      authorization: https://login.sonraisecurity.com/authorize\n      token: https://login.sonraisecurity.com/oauth/token\n      userinfo: https://login.sonraisecurity.com/userinfo\n      device_authorization: https://login.sonraisecurity.com/oauth/device/code\n      revocation: https://login.sonraisecurity.com/oauth/revoke\n      jwks: https://login.sonraisecurity.com/.well-known/jwks.json\n    scopes_supported:\n      - openid\n      - profile\n      - offline_access\n      - email\n    code_challenge_methods_supported: [S256, plain]\n    evidence: observed 302 to login.sonraisecurity.com/authorize with scope=openid+profile\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    applies_to: Sonrai GraphQL API (https://app.sonraisecurity.com/graphql)\n    evidence: >-\n      CPF developer docs document a GraphQL API; the app.sonraisecurity.com/graphql\n      endpoint responds (405 to unauthenticated\
  \ probe) and the reference is gated\n      behind the Auth0 login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonrai-security/refs/heads/main/authentication/sonrai-security-authentication.yml
summary_line: oauth2/openIdConnect/http · 2 schemes
tags:
- Company
- Security
- Cloud Security
- Identity and Access Management
- CIEM
- Cloud Permissions
- Least Privilege
- GraphQL
- IAM
---
