---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Blueleaf Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BlueLeaf secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BlueLeaf
provider_slug: blueleaf
scheme_count: 2
schemes:
- issuer: https://secure.blueleaf.com
  name: OpenIDConnect
  openIdConnectUrl: https://secure.blueleaf.com/.well-known/openid-configuration
  sources:
  - well-known/blueleaf-openid-configuration.json
  type: openIdConnect
- endpoints:
    introspection: https://secure.blueleaf.com/oauth/introspect
    jwks_uri: https://secure.blueleaf.com/.well-known/jwks.json
    revocation: https://secure.blueleaf.com/oauth/revoke
    userinfo: https://secure.blueleaf.com/oauth/userinfo
  flows:
  - authorizationUrl: https://secure.blueleaf.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://secure.blueleaf.com/oauth/token
    scopes:
    - openid
    - email
    - profile
    tokenUrl: https://secure.blueleaf.com/oauth/token
  id_token_signing_alg:
  - RS256
  name: OAuth2
  sources:
  - well-known/blueleaf-openid-configuration.json
  type: oauth2
slug: blueleaf-authentication
source_filename: blueleaf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://secure.blueleaf.com/.well-known/openid-configuration\ndocs: https://www.blueleaf.com/developer/\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256, plain]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://secure.blueleaf.com/.well-known/openid-configuration\n  issuer: https://secure.blueleaf.com\n  sources: [well-known/blueleaf-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.blueleaf.com/oauth/authorize\n    tokenUrl: https://secure.blueleaf.com/oauth/token\n    refreshUrl: https://secure.blueleaf.com/oauth/token\n    scopes: [openid, email, profile]\n  endpoints:\n    userinfo: https://secure.blueleaf.com/oauth/userinfo\n    introspection: https://secure.blueleaf.com/oauth/introspect\n\
  \    revocation: https://secure.blueleaf.com/oauth/revoke\n    jwks_uri: https://secure.blueleaf.com/.well-known/jwks.json\n  id_token_signing_alg: [RS256]\n  sources: [well-known/blueleaf-openid-configuration.json]\nnotes: >-\n  Blueleaf operates an OAuth 2.0 / OpenID Connect provider at secure.blueleaf.com\n  (authorization_code grant with refresh tokens, PKCE S256). Additional data-access\n  API details (account balances, holdings, transactions) are gated behind sales\n  contact and not publicly documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueleaf/refs/heads/main/authentication/blueleaf-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Wealth Management
- Fintech
- Financial Advisors
- Investment Reporting
- Account Aggregation
- Client Portal
- OAuth
- OpenID Connect
---
