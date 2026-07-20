---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Flow Engineering Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Flow Engineering secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Flow Engineering
provider_slug: flow-engineering
scheme_count: 1
schemes:
- authorization_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/authorize
  end_session_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/logout
  id_token_signing_alg: RS256
  issuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS
  jwks_uri: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS/.well-known/jwks.json
  name: Cognito OAuth2 / OIDC
  provider: AWS Cognito (user pool eu-west-2_iODQDOUFS, region eu-west-2)
  response_types_supported:
  - code
  - token
  revocation_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/revoke
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  token_format: JWT bearer (RS256) presented to the GraphQL API as Authorization header
  token_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/token
  type: oauth2
  userinfo_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/userInfo
slug: flow-engineering-authentication
source_filename: flow-engineering-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS/.well-known/openid-configuration\ndocs: https://flowengineering.com/security\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, implicit]\n  provider: AWS Cognito\n  enterprise_sso: [SAML, SCIM]\nschemes:\n- name: Cognito OAuth2 / OIDC\n  type: oauth2\n  provider: AWS Cognito (user pool eu-west-2_iODQDOUFS, region eu-west-2)\n  issuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS\n  authorization_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/authorize\n  token_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/token\n  userinfo_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/userInfo\n  revocation_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/revoke\n  end_session_url: https://flowengineering.auth.eu-west-2.amazoncognito.com/logout\n\
  \  jwks_uri: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS/.well-known/jwks.json\n  response_types_supported: [code, token]\n  id_token_signing_alg: RS256\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  token_format: JWT bearer (RS256) presented to the GraphQL API as Authorization header\nenterprise:\n  note: >-\n    The /security page documents SAML SSO and SCIM provisioning with granular role-based access\n    control for enterprise tenants, layered on top of the Cognito identity backend.\napi_endpoint:\n  url: https://api.flowengineering.com/v1/graphql\n  auth: OAuth2 bearer (Cognito-issued JWT); unauthenticated requests return\n    access-denied (\"Authentication hook unauthorized this request\")\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flow-engineering/refs/heads/main/authentication/flow-engineering-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Software Development
- Hardware Engineering
- Requirements Management
- Systems Engineering
- MBSE
- AI Agents
- CAD
- Product Lifecycle Management
- GraphQL
---
