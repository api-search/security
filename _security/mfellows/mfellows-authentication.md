---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Mfellows Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MFellows secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MFellows
provider_slug: mfellows
scheme_count: 2
schemes:
- issuer: https://moneyfellows.com/
  name: openIdConnect
  openIdConnectUrl: https://moneyfellows.com/.well-known/openid-configuration
  sources:
  - well-known/mfellows-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/authorize
    code_challenge_methods:
    - plain
    - S256
    endSessionUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/signout
    flow: authorizationCode
    revocationUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/revoke
    tokenUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
  name: oauth2
  sources:
  - well-known/mfellows-oauth-authorization-server.json
  type: oauth2
slug: mfellows-authentication
source_filename: mfellows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://moneyfellows.com/.well-known/openid-configuration\ndocs: https://moneyfellows.com/.well-known/openid-configuration\nnotes: >-\n  Derived from the published OpenID Connect / OAuth 2.0 discovery document on the\n  moneyfellows.com domain. This authorization server is the Umbraco CMS Content\n  Delivery API member-auth server that backs the website; Money Fellows publishes\n  no separate developer/product API. Authorization Code flow with PKCE (S256) and\n  refresh tokens; RS256-signed ID tokens.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  refresh_tokens: true\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://moneyfellows.com/.well-known/openid-configuration\n  issuer: https://moneyfellows.com/\n  sources:\n  - well-known/mfellows-openid-configuration.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/token\n    revocationUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/revoke\n    endSessionUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/signout\n    code_challenge_methods:\n    - plain\n    - S256\n    token_endpoint_auth_methods:\n    - client_secret_basic\n    - client_secret_post\n  sources:\n  - well-known/mfellows-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mfellows/refs/heads/main/authentication/mfellows-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Fintech
- Financial Services
- Savings
- Lending
- ROSCA
- Payments
- Egypt
- Mobile
- Consumer Finance
---
