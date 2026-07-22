---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: River Financial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: River Financial secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: River Financial
provider_slug: river-financial
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://river.com/oauth2/authorize
    flow: authorizationCode
    pkce_required: S256
    refresh: true
    tokenUrl: https://river.com/oauth2/token
  name: OAuth2
  sources:
  - https://river.com/.well-known/openid-configuration
  type: oauth2
- issuer: https://river.com
  jwks_uri: https://river.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://river.com/.well-known/openid-configuration
  sources:
  - https://river.com/.well-known/openid-configuration
  type: openIdConnect
  userinfo_endpoint: https://river.com/oauth2/userinfo
slug: river-financial-authentication
source_filename: river-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://river.com/.well-known/openid-configuration\ndocs: https://river.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - ES256\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://river.com/oauth2/authorize\n    tokenUrl: https://river.com/oauth2/token\n    refresh: true\n    pkce_required: S256\n  sources:\n  - https://river.com/.well-known/openid-configuration\n- name: OpenIDConnect\n  type: openIdConnect\n  issuer: https://river.com\n  openIdConnectUrl: https://river.com/.well-known/openid-configuration\n  userinfo_endpoint: https://river.com/oauth2/userinfo\n  jwks_uri: https://river.com/.well-known/jwks.json\n  sources:\n  - https://river.com/.well-known/openid-configuration\nnotes: >-\n\
  \  River exposes an OAuth 2.0 authorization-code + PKCE (S256) authorization\n  server with OIDC discovery. ID tokens are signed with ES256. Client\n  authentication at the token endpoint is client_secret_basic. A GraphQL API\n  is served at https://river.com/api (bearer access token).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/river-financial/refs/heads/main/authentication/river-financial-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Bitcoin Services
- Cryptocurrency
- Financial Services
- Banking
- OAuth
- API
---
