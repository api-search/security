---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Affiniti Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
- refreshToken
- password
- tokenExchange
- jwtBearer
overview: Affiniti secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, deviceCode, refreshToken, password, tokenExchange, and jwtBearer flow(s).
provider_name: Affiniti
provider_slug: affiniti
scheme_count: 2
schemes:
- authorization_endpoint: https://cms-login.extu.com/authorize
  backchannel_authentication_endpoint: https://cms-login.extu.com/bc-authorize
  device_authorization_endpoint: https://cms-login.extu.com/oauth/device/code
  dpop_signing_alg_values:
  - ES256
  id_token_signing_alg_values:
  - HS256
  - RS256
  - PS256
  issuer: https://cms-login.extu.com/
  jwks_uri: https://cms-login.extu.com/.well-known/jwks.json
  name: extu-cms-auth0
  openIdConnectUrl: https://cms-login.extu.com/.well-known/openid-configuration
  registration_endpoint: https://cms-login.extu.com/oidc/register
  revocation_endpoint: https://cms-login.extu.com/oauth/revoke
  scope_count: 14
  serves: Extu CMS application at https://app.extu.com
  sources:
  - well-known/affiniti-cms-login-openid-configuration.json
  token_endpoint: https://cms-login.extu.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://cms-login.extu.com/userinfo
- authorization_endpoint: https://pexp-login.extu.com/authorize
  backchannel_authentication_endpoint: https://pexp-login.extu.com/bc-authorize
  device_authorization_endpoint: https://pexp-login.extu.com/oauth/device/code
  dpop_signing_alg_values:
  - ES256
  end_session_endpoint: https://pexp-login.extu.com/oidc/logout
  id_token_signing_alg_values:
  - HS256
  - RS256
  - PS256
  issuer: https://pexp-login.extu.com/
  jwks_uri: https://pexp-login.extu.com/.well-known/jwks.json
  name: extu-pexp-auth0
  openIdConnectUrl: https://pexp-login.extu.com/.well-known/openid-configuration
  registration_endpoint: https://pexp-login.extu.com/oidc/register
  revocation_endpoint: https://pexp-login.extu.com/oauth/revoke
  scope_count: 14
  serves: Extu Partner Experience Platform (PEXP)
  sources:
  - well-known/affiniti-pexp-login-openid-configuration.json
  token_endpoint: https://pexp-login.extu.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://pexp-login.extu.com/userinfo
slug: affiniti-authentication
source_filename: affiniti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://cms-login.extu.com/.well-known/openid-configuration and\n  https://pexp-login.extu.com/.well-known/openid-configuration\nnote: >-\n  Derived from the two OpenID Connect discovery documents the provider serves, not from an\n  OpenAPI — Affiniti/Extu publishes no API contract. These describe how a HUMAN signs in to the\n  Extu applications (the CMS at app.extu.com and the Partner Experience Platform), not a\n  documented developer authentication flow: there is no public client registration guide, no API\n  key issuance, and no documented audience for a third-party integration. Both tenants are Auth0\n  custom domains on extu.com hosts (the auth0.com grant-type URNs in grant_types_supported are the\n  tell), so the metadata is Auth0's stock tenant configuration served under Extu's own domain.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, clientCredentials,\
  \ deviceCode, refreshToken, password, tokenExchange, jwtBearer]\n  pkce: [S256, plain]\n  mfa: true\n  dpop: true\n  developer_facing: false\nschemes:\n- name: extu-cms-auth0\n  type: openIdConnect\n  openIdConnectUrl: https://cms-login.extu.com/.well-known/openid-configuration\n  issuer: https://cms-login.extu.com/\n  authorization_endpoint: https://cms-login.extu.com/authorize\n  token_endpoint: https://cms-login.extu.com/oauth/token\n  userinfo_endpoint: https://cms-login.extu.com/userinfo\n  jwks_uri: https://cms-login.extu.com/.well-known/jwks.json\n  registration_endpoint: https://cms-login.extu.com/oidc/register\n  revocation_endpoint: https://cms-login.extu.com/oauth/revoke\n  device_authorization_endpoint: https://cms-login.extu.com/oauth/device/code\n  backchannel_authentication_endpoint: https://cms-login.extu.com/bc-authorize\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  id_token_signing_alg_values: [HS256, RS256, PS256]\n\
  \  dpop_signing_alg_values: [ES256]\n  scope_count: 14\n  serves: Extu CMS application at https://app.extu.com\n  sources: [well-known/affiniti-cms-login-openid-configuration.json]\n- name: extu-pexp-auth0\n  type: openIdConnect\n  openIdConnectUrl: https://pexp-login.extu.com/.well-known/openid-configuration\n  issuer: https://pexp-login.extu.com/\n  authorization_endpoint: https://pexp-login.extu.com/authorize\n  token_endpoint: https://pexp-login.extu.com/oauth/token\n  userinfo_endpoint: https://pexp-login.extu.com/userinfo\n  jwks_uri: https://pexp-login.extu.com/.well-known/jwks.json\n  registration_endpoint: https://pexp-login.extu.com/oidc/register\n  revocation_endpoint: https://pexp-login.extu.com/oauth/revoke\n  device_authorization_endpoint: https://pexp-login.extu.com/oauth/device/code\n  backchannel_authentication_endpoint: https://pexp-login.extu.com/bc-authorize\n  end_session_endpoint: https://pexp-login.extu.com/oidc/logout\n  token_endpoint_auth_methods: [client_secret_basic,\
  \ client_secret_post, private_key_jwt, none]\n  id_token_signing_alg_values: [HS256, RS256, PS256]\n  dpop_signing_alg_values: [ES256]\n  scope_count: 14\n  serves: Extu Partner Experience Platform (PEXP)\n  sources: [well-known/affiniti-pexp-login-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affiniti/refs/heads/main/authentication/affiniti-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Channel Marketing
- Marketing Automation
- Through-Channel Marketing
- Partner Marketing
- Incentives
- Loyalty
- Rebates
- Rewards
- B2B SaaS
---
