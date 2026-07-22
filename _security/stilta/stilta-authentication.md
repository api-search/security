---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Stilta Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Stilta secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Stilta
provider_slug: stilta
scheme_count: 2
schemes:
- issuer: https://auth.stilta.com
  name: OpenIDConnect
  openIdConnectUrl: https://auth.stilta.com/.well-known/openid-configuration
  sources:
  - well-known/stilta-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.stilta.com/propelauth/oauth/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    idTokenSigningAlg:
    - RS256
    jwksUri: https://auth.stilta.com/.well-known/jwks.json
    tokenEndpointAuthMethods:
    - client_secret_basic
    - client_secret_post
    tokenUrl: https://auth.stilta.com/propelauth/oauth/token
    userinfoUrl: https://auth.stilta.com/propelauth/oauth/userinfo
  name: OAuth2
  sources:
  - well-known/stilta-openid-configuration.json
  type: oauth2
slug: stilta-authentication
source_filename: stilta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.stilta.com/.well-known/openid-configuration\ndocs: https://auth.stilta.com/en/login\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  provider: PropelAuth\n  note: >-\n    OpenID Connect identity surface for the Stilta platform (SSO / user login),\n    not a documented developer API authorization surface. Discovered via the\n    published /.well-known/openid-configuration document.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  issuer: https://auth.stilta.com\n  openIdConnectUrl: https://auth.stilta.com/.well-known/openid-configuration\n  sources:\n  - well-known/stilta-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.stilta.com/propelauth/oauth/authorize\n    tokenUrl: https://auth.stilta.com/propelauth/oauth/token\n    userinfoUrl: https://auth.stilta.com/propelauth/oauth/userinfo\n\
  \    jwksUri: https://auth.stilta.com/.well-known/jwks.json\n    codeChallengeMethods:\n    - S256\n    tokenEndpointAuthMethods:\n    - client_secret_basic\n    - client_secret_post\n    idTokenSigningAlg:\n    - RS256\n  sources:\n  - well-known/stilta-openid-configuration.json\nscopes:\n- scope: openid\n  description: OpenID Connect authentication\n- scope: email\n  description: Access to the user's email address\n- scope: profile\n  description: Access to the user's basic profile (first_name, last_name, picture_url)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stilta/refs/heads/main/authentication/stilta-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Patents
- Intellectual Property
- Legal Tech
- Artificial Intelligence
- Agentic AI
- Patent Search
- Prior Art
---
