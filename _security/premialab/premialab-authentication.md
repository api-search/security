---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Premialab Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- clientCredentials
- refreshToken
overview: PremiaLab secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, clientCredentials, and refreshToken flow(s).
provider_name: PremiaLab
provider_slug: premialab
scheme_count: 2
schemes:
- issuer: https://sso.plbtech.com
  name: PremiaLabOIDC
  openIdConnectUrl: https://sso.plbtech.com/.well-known/openid-configuration
  sources:
  - well-known/premialab-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://sso.plbtech.com/oauth2/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://sso.plbtech.com/oauth2/v1/token
  - deviceAuthorizationUrl: https://sso.plbtech.com/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://sso.plbtech.com/oauth2/v1/token
  - flow: refreshToken
    tokenUrl: https://sso.plbtech.com/oauth2/v1/token
  name: PremiaLabOAuth2
  sources:
  - well-known/premialab-openid-configuration.json
  type: oauth2
slug: premialab-authentication
source_filename: premialab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  Live probe of https://api.premialab.com (HTTP 302 to Okta authorize) and the\n  OIDC discovery document at https://sso.plbtech.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, deviceCode, clientCredentials, refreshToken]\n  api_key_in: []\n  notes: >-\n    The PremiaLab client API is not publicly documented and requires an\n    OAuth2/OIDC access token issued by the PremiaLab Tech (plbtech.com) Okta\n    authorization server. Access is provisioned for institutional clients; no\n    self-service developer signup is published.\nschemes:\n  - name: PremiaLabOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://sso.plbtech.com/.well-known/openid-configuration\n    issuer: https://sso.plbtech.com\n    sources: [well-known/premialab-openid-configuration.json]\n  - name: PremiaLabOAuth2\n    type: oauth2\n    sources: [well-known/premialab-openid-configuration.json]\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sso.plbtech.com/oauth2/v1/authorize\n        tokenUrl: https://sso.plbtech.com/oauth2/v1/token\n        pkce: S256\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://sso.plbtech.com/oauth2/v1/device/authorize\n        tokenUrl: https://sso.plbtech.com/oauth2/v1/token\n      - flow: refreshToken\n        tokenUrl: https://sso.plbtech.com/oauth2/v1/token\nendpoints:\n  authorization: https://sso.plbtech.com/oauth2/v1/authorize\n  token: https://sso.plbtech.com/oauth2/v1/token\n  userinfo: https://sso.plbtech.com/oauth2/v1/userinfo\n  jwks: https://sso.plbtech.com/oauth2/v1/keys\n  introspection: https://sso.plbtech.com/oauth2/v1/introspect\n  revocation: https://sso.plbtech.com/oauth2/v1/revoke\n  end_session: https://sso.plbtech.com/oauth2/v1/logout\n  registration: https://sso.plbtech.com/oauth2/v1/clients\n  pushed_authorization_request: https://sso.plbtech.com/oauth2/v1/par\ntoken_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\nid_token_signing_alg: [RS256]\ndpop_supported: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premialab/refs/heads/main/authentication/premialab-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Financial Services
- Fintech
- Investment Management
- Risk Analytics
- Portfolio Analytics
- Quantitative Investment Strategies
- Factor Investing
---
