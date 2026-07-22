---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Manifest Law Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Manifest Law secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Manifest Law
provider_slug: manifest-law
scheme_count: 2
schemes:
- issuer: https://app.manifestlaw.com/api/auth
  name: OpenIDConnect
  openIdConnectUrl: https://app.manifestlaw.com/.well-known/openid-configuration
  sources:
  - well-known/manifest-law-openid-configuration.json
  type: openIdConnect
- authorizationUrl: https://app.manifestlaw.com/api/auth/oauth2/authorize
  code_challenge_methods:
  - S256
  endSessionUrl: https://app.manifestlaw.com/api/auth/oauth2/end-session
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  id_token_signing_alg:
  - HS256
  introspectionUrl: https://app.manifestlaw.com/api/auth/oauth2/introspect
  issuer: https://app.manifestlaw.com/api/auth
  name: OAuth2
  revocationUrl: https://app.manifestlaw.com/api/auth/oauth2/revoke
  sources:
  - well-known/manifest-law-oauth-authorization-server.json
  tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfoUrl: https://app.manifestlaw.com/api/auth/oauth2/userinfo
slug: manifest-law-authentication
source_filename: manifest-law-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.manifestlaw.com/.well-known/openid-configuration\ndocs: https://app.manifestlaw.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  pkce: [S256]\n  notes: >-\n    Manifest Law (ManifestOS) publishes a standards-based OAuth 2.0 / OpenID Connect\n    authorization server at https://app.manifestlaw.com/api/auth. Discovery documents\n    are served at /.well-known/openid-configuration and /.well-known/oauth-authorization-server.\n    Dynamic client management is supported via the oauth_clients:manage scope, and an\n    \"api\" scope gates programmatic API access.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://app.manifestlaw.com/.well-known/openid-configuration\n  issuer: https://app.manifestlaw.com/api/auth\n  sources: [well-known/manifest-law-openid-configuration.json]\n- name:\
  \ OAuth2\n  type: oauth2\n  issuer: https://app.manifestlaw.com/api/auth\n  authorizationUrl: https://app.manifestlaw.com/api/auth/oauth2/authorize\n  tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token\n  introspectionUrl: https://app.manifestlaw.com/api/auth/oauth2/introspect\n  revocationUrl: https://app.manifestlaw.com/api/auth/oauth2/revoke\n  userinfoUrl: https://app.manifestlaw.com/api/auth/oauth2/userinfo\n  endSessionUrl: https://app.manifestlaw.com/api/auth/oauth2/end-session\n  flows: [authorizationCode, clientCredentials, refreshToken]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [HS256]\n  sources: [well-known/manifest-law-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manifest-law/refs/heads/main/authentication/manifest-law-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Legal
- Legal Tech
- Case Management
- Communication
- OAuth
- OpenID Connect
---
