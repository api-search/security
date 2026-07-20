---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Jit Fka Cbrix Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- deviceCode
- tokenExchange
- refreshToken
overview: Jit (fka Cbrix) secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, deviceCode, tokenExchange, and refreshToken flow(s).
provider_name: Jit (fka Cbrix)
provider_slug: jit-fka-cbrix
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: API requests to api.jit.io are authorized with a Bearer JWT. Clients obtain the JWT by POSTing their Client ID and Secret to the credentials endpoint (https://api.jit.io/authentication/login). The issued token is valid for 24 hours, after which the client must re-authenticate.
  name: BearerJWT
  scheme: bearer
  sources:
  - https://docs.jit.io/reference/credentials
  type: http
- authorization_server: https://auth.jit.io
  description: Jit runs a full OAuth2 / OpenID Connect authorization server at auth.jit.io. Machine-to-machine API access uses the client_credentials grant (Client ID + Secret issued under Settings -> Users & Permissions -> API Tokens). Interactive and device flows are also supported.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.jit.io/oauth/token
  - authorizationUrl: https://auth.jit.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.jit.io/oauth/token
  - deviceAuthorizationUrl: https://auth.jit.io/oauth/device/authorize
    flow: deviceCode
    tokenUrl: https://auth.jit.io/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  - ES256
  name: OAuth2
  registration_endpoint: https://auth.jit.io/oauth/dcr/register
  sources:
  - https://auth.jit.io/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: jit-fka-cbrix-authentication
source_filename: jit-fka-cbrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.jit.io/reference/credentials\ndocs: https://docs.jit.io/docs/managing-users\ndiscovery: https://auth.jit.io/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  - deviceCode\n  - tokenExchange\n  - refreshToken\n  bearer_format: JWT\nschemes:\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    API requests to api.jit.io are authorized with a Bearer JWT. Clients obtain the\n    JWT by POSTing their Client ID and Secret to the credentials endpoint\n    (https://api.jit.io/authentication/login). The issued token is valid for 24\n    hours, after which the client must re-authenticate.\n  sources:\n  - https://docs.jit.io/reference/credentials\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Jit runs a full OAuth2 / OpenID Connect authorization server\
  \ at auth.jit.io.\n    Machine-to-machine API access uses the client_credentials grant (Client ID +\n    Secret issued under Settings -> Users & Permissions -> API Tokens). Interactive\n    and device flows are also supported.\n  authorization_server: https://auth.jit.io\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.jit.io/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.jit.io/oauth/authorize\n    tokenUrl: https://auth.jit.io/oauth/token\n    pkce: S256\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.jit.io/oauth/device/authorize\n    tokenUrl: https://auth.jit.io/oauth/token\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  - ES256\n  registration_endpoint:\
  \ https://auth.jit.io/oauth/dcr/register\n  sources:\n  - https://auth.jit.io/.well-known/openid-configuration\nroles:\n  description: >-\n    API tokens are created against a user role; the token inherits that role's\n    permissions.\n  values:\n  - Admin\n  - Engineering Manager\n  - Member\n  - Developer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jit-fka-cbrix/refs/heads/main/authentication/jit-fka-cbrix-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Cybersecurity
- Application Security
- DevSecOps
- ASPM
- Security
- Vulnerability Management
- API
---
