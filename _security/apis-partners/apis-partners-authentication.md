---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Apis Partners Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Apis Partners secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Apis Partners
provider_slug: apis-partners
scheme_count: 2
schemes:
- issuer: https://www.apis.pe/
  name: openIdConnect
  openIdConnectUrl: https://apis.pe/.well-known/openid-configuration
  sources:
  - well-known/apis-partners-openid-configuration.json
  type: openIdConnect
- endpoints:
    end_session: https://www.apis.pe/umbraco/delivery/api/v1/security/member/signout
    jwks_uri: https://www.apis.pe/.well-known/jwks
    revocation: https://www.apis.pe/umbraco/delivery/api/v1/security/member/revoke
    userinfo: https://www.apis.pe/umbraco/delivery/api/v1/security/member/userinfo
  flows:
  - authorizationUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    refreshUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token
    scopes:
    - openid
    - offline_access
    tokenUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token
  - flow: clientCredentials
    scopes: []
    tokenUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token
  name: oauth2
  sources:
  - well-known/apis-partners-openid-configuration.json
  type: oauth2
slug: apis-partners-authentication
source_filename: apis-partners-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://apis.pe/.well-known/openid-configuration\nnote: >-\n  Apis Partners publishes no business/developer API. The only machine-readable auth\n  surface at the domain is the Umbraco CMS Delivery API member authentication, advertised\n  via a valid OpenID Connect discovery document. Captured faithfully from that document.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  grant_types: [authorization_code, refresh_token, client_credentials]\n  pkce: [plain, S256]\n  token_endpoint_auth_methods: [client_secret_post, private_key_jwt, client_secret_basic]\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://apis.pe/.well-known/openid-configuration\n  issuer: https://www.apis.pe/\n  sources: [well-known/apis-partners-openid-configuration.json]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/authorize\n\
  \    tokenUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token\n    refreshUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token\n    scopes: [openid, offline_access]\n  - flow: clientCredentials\n    tokenUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token\n    scopes: []\n  endpoints:\n    userinfo: https://www.apis.pe/umbraco/delivery/api/v1/security/member/userinfo\n    revocation: https://www.apis.pe/umbraco/delivery/api/v1/security/member/revoke\n    end_session: https://www.apis.pe/umbraco/delivery/api/v1/security/member/signout\n    jwks_uri: https://www.apis.pe/.well-known/jwks\n  sources: [well-known/apis-partners-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-partners/refs/heads/main/authentication/apis-partners-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Venture
- Private Equity
- Fintech
- Financial Services
- Payments
- Investor
- Emerging Markets
---
