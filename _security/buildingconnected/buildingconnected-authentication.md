---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Buildingconnected Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Buildingconnected secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Buildingconnected
provider_slug: buildingconnected
scheme_count: 2
schemes:
- authorization_endpoint: https://developer.api.autodesk.com/authentication/v2/authorize
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://developer.api.autodesk.com/authentication/v2/introspect
  issuer: https://developer.api.autodesk.com
  jwks_uri: https://developer.api.autodesk.com/authentication/v2/keys
  name: APS OAuth 2.0
  revocation_endpoint: https://developer.api.autodesk.com/authentication/v2/revoke
  sources:
  - well-known/buildingconnected-openid-configuration.json
  token_endpoint: https://developer.api.autodesk.com/authentication/v2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- name: APS OpenID Connect
  openIdConnectUrl: https://developer.api.autodesk.com/.well-known/openid-configuration
  sources:
  - well-known/buildingconnected-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://api.userprofile.autodesk.com/userinfo
slug: buildingconnected-authentication
source_filename: buildingconnected-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.api.autodesk.com/.well-known/openid-configuration\ndocs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/overview/\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  pkce: true\n  pkce_methods: [S256]\n  provider: Autodesk Platform Services (APS) shared OAuth 2.0 / OIDC authorization server\nschemes:\n- name: APS OAuth 2.0\n  type: oauth2\n  issuer: https://developer.api.autodesk.com\n  authorization_endpoint: https://developer.api.autodesk.com/authentication/v2/authorize\n  token_endpoint: https://developer.api.autodesk.com/authentication/v2/token\n  revocation_endpoint: https://developer.api.autodesk.com/authentication/v2/revoke\n  introspection_endpoint: https://developer.api.autodesk.com/authentication/v2/introspect\n  jwks_uri: https://developer.api.autodesk.com/authentication/v2/keys\n  grant_types: [authorization_code, client_credentials,\
  \ refresh_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  sources: [well-known/buildingconnected-openid-configuration.json]\n- name: APS OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://developer.api.autodesk.com/.well-known/openid-configuration\n  userinfo_endpoint: https://api.userprofile.autodesk.com/userinfo\n  sources: [well-known/buildingconnected-openid-configuration.json]\nnotes: >-\n  The BuildingConnected API does not run its own authorization server; it authenticates\n  through the platform-wide APS OAuth 2.0 service (two-legged client_credentials and\n  three-legged authorization_code with PKCE). Endpoints and grant types captured verbatim\n  from the live authorization-server discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildingconnected/refs/heads/main/authentication/buildingconnected-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Construction
- Preconstruction
- Bid Management
- Construction Technology
- Autodesk
- Autodesk Platform Services
- Subcontractor Management
---
