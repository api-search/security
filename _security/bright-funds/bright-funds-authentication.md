---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bright Funds Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Bright Funds secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Bright Funds
provider_slug: bright-funds
scheme_count: 2
schemes:
- name: OpenIDConnect
  openIdConnectUrl: https://www.brightfunds.org/.well-known/openid-configuration
  sources:
  - well-known/bright-funds-openid-configuration.json
  type: openIdConnect
- authorizationUrl: https://www.brightfunds.org/oauth/authorize
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  - refreshToken
  id_token_signing_alg:
  - RS256
  introspectionUrl: https://www.brightfunds.org/oauth/introspect
  issuer: https://www.brightfunds.org/
  jwksUrl: https://www.brightfunds.org/oauth/discovery/keys
  name: OAuth2
  revocationUrl: https://www.brightfunds.org/oauth/revoke
  sources:
  - well-known/bright-funds-oauth-authorization-server.json
  subject_types:
  - pairwise
  tokenUrl: https://www.brightfunds.org/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfoUrl: https://www.brightfunds.org/oauth/userinfo
slug: bright-funds-authentication
source_filename: bright-funds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.brightfunds.org/.well-known/openid-configuration\ndocs: https://www.brightfunds.org/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, implicit]\n  oidc: true\n  issuer: https://www.brightfunds.org/\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.brightfunds.org/.well-known/openid-configuration\n  sources: [well-known/bright-funds-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  issuer: https://www.brightfunds.org/\n  authorizationUrl: https://www.brightfunds.org/oauth/authorize\n  tokenUrl: https://www.brightfunds.org/oauth/token\n  revocationUrl: https://www.brightfunds.org/oauth/revoke\n  introspectionUrl: https://www.brightfunds.org/oauth/introspect\n  userinfoUrl: https://www.brightfunds.org/oauth/userinfo\n  jwksUrl: https://www.brightfunds.org/oauth/discovery/keys\n  flows:\
  \ [authorizationCode, clientCredentials, implicit, refreshToken]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  subject_types: [pairwise]\n  sources: [well-known/bright-funds-oauth-authorization-server.json]\nnotes: >-\n  Discovered from the live OIDC/OAuth 2.0 authorization-server metadata; no public OpenAPI or\n  developer portal documents the API surface, so schemes are captured from discovery rather than\n  derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-funds/refs/heads/main/authentication/bright-funds-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Workplace Giving
- Corporate Social Responsibility
- Employee Engagement
- Nonprofits
- Grants Management
- Donations
- Volunteering
- OAuth
- OpenID Connect
---
