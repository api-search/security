---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Joor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- deviceCode
- ciba
- implicit
overview: Joor secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, deviceCode, ciba, and implicit flow(s).
provider_name: Joor
provider_slug: joor
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  - plain
  endpoints:
    authorization: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/auth
    end_session: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/logout
    introspection: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token/introspect
    token: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token
    userinfo: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id_token_signing_alg_values:
  - RS256
  - ES256
  - PS256
  - RS384
  - ES384
  - PS384
  - RS512
  - ES512
  - PS512
  - HS256
  - HS384
  - HS512
  issuer: https://auth.jooraccess.com/auth/realms/joor
  name: openIdConnect
  openIdConnectUrl: https://auth.jooraccess.com/auth/realms/joor/.well-known/openid-configuration
  sources:
  - well-known/joor-openid-configuration.json
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
slug: joor-authentication
source_filename: joor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.jooraccess.com/auth/realms/joor/.well-known/openid-configuration\ndocs: https://auth.jooraccess.com/auth/realms/joor/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, password, deviceCode, ciba, implicit]\n  pkce: [S256, plain]\n  provider: Keycloak\n  gateway: Kong\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.jooraccess.com/auth/realms/joor/.well-known/openid-configuration\n  issuer: https://auth.jooraccess.com/auth/realms/joor\n  endpoints:\n    authorization: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/auth\n    token: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token\n    userinfo: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/userinfo\n    introspection: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token/introspect\n\
  \    end_session: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/logout\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  code_challenge_methods: [S256, plain]\n  id_token_signing_alg_values: [RS256, ES256, PS256, RS384, ES384, PS384, RS512, ES512, PS512, HS256, HS384, HS512]\n  sources: [well-known/joor-openid-configuration.json]\nnotes: >-\n  Auth is derived from the live Keycloak OIDC discovery document (searched), not\n  from a JOOR-published OpenAPI (none is public). client_credentials and\n  private_key_jwt/tls_client_auth support indicate machine-to-machine and\n  mTLS-capable integration clients; PKCE S256 is supported for public clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joor/refs/heads/main/authentication/joor-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Fashion
- Wholesale
- Retail
- eCommerce
- B2B
- Marketplace
- Payments
---
