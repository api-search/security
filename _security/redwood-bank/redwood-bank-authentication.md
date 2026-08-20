---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Redwood Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Redwood Bank secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Redwood Bank
provider_slug: redwood-bank
scheme_count: 2
schemes:
- issuer: https://redwoodbank.co.uk/
  name: OpenIDConnect
  openIdConnectUrl: https://www.redwoodbank.co.uk/.well-known/openid-configuration
  sources:
  - well-known/redwood-bank-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    scopes:
      offline_access: Issue a refresh token for offline access
      openid: OpenID Connect authentication
    tokenUrl: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/token
  - flow: clientCredentials
    tokenUrl: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/token
  name: OAuth2
  sources:
  - well-known/redwood-bank-openid-configuration.json
  type: oauth2
slug: redwood-bank-authentication
source_filename: redwood-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.redwoodbank.co.uk/.well-known/openid-configuration\ndocs: https://www.redwoodbank.co.uk/.well-known/openid-configuration\nnote: >-\n  Derived from the live OpenID Connect discovery document published at the\n  website root. This is the Umbraco headless-CMS \"Content Delivery API\" member\n  authentication surface (OpenIddict), which powers the marketing site's\n  member/gated-content area. Redwood Bank publishes NO Open Banking / banking\n  API and therefore no product-facing auth scheme; this is the only documented\n  authentication surface on the domain.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  pkce: true\n  pkce_methods: [S256, plain]\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.redwoodbank.co.uk/.well-known/openid-configuration\n  issuer: https://redwoodbank.co.uk/\n  sources: [well-known/redwood-bank-openid-configuration.json]\n\
  - name: OAuth2\n  type: oauth2\n  sources: [well-known/redwood-bank-openid-configuration.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/token\n    scopes:\n      openid: OpenID Connect authentication\n      offline_access: Issue a refresh token for offline access\n  - flow: clientCredentials\n    tokenUrl: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/token\nendpoints:\n  authorization_endpoint: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/authorize\n  token_endpoint: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/token\n  userinfo_endpoint: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/userinfo\n  end_session_endpoint: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/signout\n  revocation_endpoint: https://redwoodbank.co.uk/umbraco/delivery/api/v1/security/member/revoke\n\
  \  jwks_uri: https://redwoodbank.co.uk/.well-known/jwks\n  token_endpoint_auth_methods: [client_secret_post, private_key_jwt, client_secret_basic]\n  id_token_signing_alg: [RS256]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redwood-bank/refs/heads/main/authentication/redwood-bank-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial-Services
- Banking
- Business Banking
- SME
- Savings
- Commercial Mortgages
- Open Banking
- PSD2
- OBIE
- United Kingdom
---
