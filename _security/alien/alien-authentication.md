---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Alien Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Alien secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Alien
provider_slug: alien
scheme_count: 2
schemes:
- issuer: https://sso.alien-api.com
  name: AlienSSO
  openIdConnectUrl: https://sso.alien-api.com/.well-known/openid-configuration
  source: https://sso.alien-api.com/.well-known/openid-configuration
  type: openIdConnect
- flows:
  - authorizationUrl: https://sso.alien-api.com/oauth/authorize
    flow: authorizationCode
    scopes:
      openid: OpenID Connect authentication (proof-of-humanity subject)
    tokenUrl: https://sso.alien-api.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2
  source: https://sso.alien-api.com/.well-known/oauth-authorization-server
  type: oauth2
slug: alien-authentication
source_filename: alien-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://sso.alien-api.com/.well-known/openid-configuration\ndocs: https://docs.alien.org/sso-guide/oauth2-clients\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken]\n  pkce: required\n  pkce_methods: [S256]\n  token_binding: DPoP (RFC 9449, EdDSA)\n  client_type: public\n  token_endpoint_auth_methods: [none]\nschemes:\n- name: AlienSSO\n  type: openIdConnect\n  openIdConnectUrl: https://sso.alien-api.com/.well-known/openid-configuration\n  issuer: https://sso.alien-api.com\n  source: https://sso.alien-api.com/.well-known/openid-configuration\n- name: OAuth2\n  type: oauth2\n  source: https://sso.alien-api.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.alien-api.com/oauth/authorize\n    tokenUrl: https://sso.alien-api.com/oauth/token\n    scopes:\n      openid: OpenID Connect authentication (proof-of-humanity subject)\n\
  \  grant_types: [authorization_code, refresh_token]\nnotes: >-\n  Alien SSO is an OpenID Connect / OAuth 2.0 identity provider that proves human\n  uniqueness rather than legal identity. Public clients only (token_endpoint_auth\n  none) with mandatory PKCE (S256). Access tokens may be sender-constrained with\n  DPoP (RFC 9449, EdDSA). ID tokens are RS256-signed; public keys at\n  https://sso.alien-api.com/oauth/jwks. Backend services verify Alien Agent ID\n  tokens (Ed25519) via @alien-id/sso-agent-id. Any standard OIDC library works.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alien/refs/heads/main/authentication/alien-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Crypto
- Identity
- Authentication
- OAuth
- OpenID Connect
- Proof of Humanity
- Blockchain
- Solana
- Agents
---
