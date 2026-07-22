---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Graniteshares Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GraniteShares secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GraniteShares
provider_slug: graniteshares
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://bkgswebv2.azurewebsites.net/umbraco/delivery/api/v1/security/member/authorize
    code_challenge_methods:
    - plain
    - S256
    flow: authorizationCode
    scopes:
      offline_access: Issue a refresh token
      openid: OpenID Connect subject identity
    tokenUrl: https://bkgswebv2.azurewebsites.net/umbraco/delivery/api/v1/security/member/token
  id_token_signing_alg:
  - RS256
  issuer: https://bkgswebv2.azurewebsites.net/
  name: umbraco-member-oidc
  openIdConnectUrl: https://graniteshares.com/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: graniteshares-authentication
source_filename: graniteshares-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://graniteshares.com/.well-known/openid-configuration\ndocs: https://graniteshares.com/.well-known/openid-configuration\nnote: >-\n  GraniteShares publishes no developer/API program. The only machine-readable\n  auth surface discovered is the OpenID Connect / OAuth 2.0 member-authentication\n  endpoint of the site's Umbraco Delivery API (issuer\n  https://bkgswebv2.azurewebsites.net/). This profiles that discovered surface,\n  not a first-party product API.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  scopes: [openid, offline_access]\nschemes:\n- name: umbraco-member-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://graniteshares.com/.well-known/openid-configuration\n  issuer: https://bkgswebv2.azurewebsites.net/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://bkgswebv2.azurewebsites.net/umbraco/delivery/api/v1/security/member/authorize\n\
  \    tokenUrl: https://bkgswebv2.azurewebsites.net/umbraco/delivery/api/v1/security/member/token\n    code_challenge_methods: [plain, S256]\n    scopes:\n      openid: OpenID Connect subject identity\n      offline_access: Issue a refresh token\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graniteshares/refs/heads/main/authentication/graniteshares-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Fintech
- ETF
- Asset Management
- Investments
- Leveraged ETFs
- Financial Services
---
