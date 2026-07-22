---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Better Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Better secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Better
provider_slug: better
scheme_count: 1
schemes:
- authorization_endpoint: https://prod.bettermg.com/api/idp/sso
  end_session_endpoint: https://prod.idp.bettermg.com/logout
  id_token_signing_alg:
  - RS256
  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_ZQ2HayNPw
  jwks_uri: https://prod.bettermg.com/.well-known/jwks.json
  name: BetterOIDC
  openIdConnectUrl: https://better.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  - token
  revocation_endpoint: https://prod.idp.bettermg.com/oauth2/revoke
  scopes:
  - openid
  - email
  - phone
  - profile
  sources:
  - well-known/better-openid-configuration.json
  token_endpoint: https://prod.bettermg.com/api/idp/token
  token_endpoint_auth_methods:
  - none
  type: openIdConnect
  userinfo_endpoint: https://prod.idp.bettermg.com/oauth2/userInfo
slug: better-authentication
source_filename: better-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://better.com/.well-known/openid-configuration\nnote: >-\n  Better does not publish a public developer API. This profiles the consumer\n  identity provider (AWS Cognito, us-east-1) that backs sign-in at better.com,\n  discovered via its OpenID Connect metadata document.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, implicit]\n  pkce: [S256]\nschemes:\n- name: BetterOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://better.com/.well-known/openid-configuration\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_ZQ2HayNPw\n  authorization_endpoint: https://prod.bettermg.com/api/idp/sso\n  token_endpoint: https://prod.bettermg.com/api/idp/token\n  userinfo_endpoint: https://prod.idp.bettermg.com/oauth2/userInfo\n  revocation_endpoint: https://prod.idp.bettermg.com/oauth2/revoke\n  end_session_endpoint: https://prod.idp.bettermg.com/logout\n  jwks_uri: https://prod.bettermg.com/.well-known/jwks.json\n\
  \  id_token_signing_alg: [RS256]\n  response_types: [code, token]\n  pkce: [S256]\n  token_endpoint_auth_methods: [none]\n  scopes: [openid, email, phone, profile]\n  sources: [well-known/better-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better/refs/heads/main/authentication/better-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Mortgage
- Lending
- Fintech
- Real Estate
- Home Equity
- Insurance
- Financial Services
---
