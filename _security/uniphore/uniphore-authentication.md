---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Uniphore Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
- deviceCode
- tokenExchange
overview: Uniphore secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, refreshToken, deviceCode, and tokenExchange flow(s).
provider_name: Uniphore
provider_slug: uniphore
scheme_count: 3
schemes:
- backchannel_logout: true
  code_challenge_methods:
  - S256
  - plain
  dpop: true
  endpoints:
    authorization: https://uniphore.us.auth0.com/authorize
    device_authorization: https://uniphore.us.auth0.com/oauth/device/code
    jwks: well-known/uniphore-jwks.json
    registration: https://uniphore.us.auth0.com/oidc/register
    revocation: https://uniphore.us.auth0.com/oauth/revoke
    token: https://uniphore.us.auth0.com/oauth/token
    userinfo: https://uniphore.us.auth0.com/userinfo
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_alg:
  - RS256
  - HS256
  - PS256
  issuer: https://uniphore.us.auth0.com/
  name: openIdConnect
  openIdConnectUrl: https://uniphore.us.auth0.com/.well-known/openid-configuration
  provider: Auth0 (Uniphore-dedicated tenant)
  sources:
  - well-known/uniphore-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- bearerFormat: JWT
  description: 'Machine-to-machine access token for the Business AI Cloud (BAIC) platform API. Exchange a client_id / client_secret pair at the deployment''s forge-user-management service, then present the returned access_token as an Authorization: Bearer header on every platform API call.'
  header: 'Authorization: Bearer <token>'
  name: m2mBearer
  response_field: access_token
  scheme: bearer
  sources:
  - https://uniphore.github.io/baic-docs/
  token_endpoint_path: /auth/m2m-token
  token_request_params:
  - client_id
  - client_secret
  type: http
- configurable: true
  description: BAIC deployments support enterprise OIDC single sign-on, configured through the forge-user-management service (oidcSso.oauthBaseUrl) and an oidc-secrets Kubernetes Secret. The identity provider is customer-supplied.
  name: oidcSso
  sources:
  - https://uniphore.github.io/baic-docs/
  type: openIdConnect
slug: uniphore-authentication
source_filename: uniphore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://uniphore.us.auth0.com/.well-known/openid-configuration\ndocs: https://uniphore.github.io/baic-docs/\nnote: >-\n  Uniphore publishes no OpenAPI, so this profile is not derived from\n  securitySchemes. It is assembled from two real, fetched sources: (1) the\n  anonymous OIDC / RFC 8414 discovery document served by Uniphore's dedicated\n  Auth0 identity tenant (uniphore.us.auth0.com), saved verbatim under\n  well-known/, and (2) the public BAIC Installation Guide, which documents the\n  machine-to-machine token exchange and the Bearer scheme used against the\n  Business AI Cloud platform API.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  - refreshToken\n  - deviceCode\n  - tokenExchange\n  bearer_format: JWT\n  pkce: true\n  mtls: false\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://uniphore.us.auth0.com/.well-known/openid-configuration\n\
  \  issuer: https://uniphore.us.auth0.com/\n  provider: Auth0 (Uniphore-dedicated tenant)\n  endpoints:\n    authorization: https://uniphore.us.auth0.com/authorize\n    token: https://uniphore.us.auth0.com/oauth/token\n    userinfo: https://uniphore.us.auth0.com/userinfo\n    jwks: well-known/uniphore-jwks.json\n    revocation: https://uniphore.us.auth0.com/oauth/revoke\n    registration: https://uniphore.us.auth0.com/oidc/register\n    device_authorization: https://uniphore.us.auth0.com/oauth/device/code\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n\
  \  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  code_challenge_methods:\n  - S256\n  - plain\n  id_token_signing_alg: [RS256, HS256, PS256]\n  dpop: true\n  backchannel_logout: true\n  sources:\n  - well-known/uniphore-openid-configuration.json\n- name: m2mBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Machine-to-machine access token for the Business AI Cloud (BAIC) platform\n    API. Exchange a client_id / client_secret pair at the deployment's\n    forge-user-management service, then present the returned access_token as\n    an Authorization: Bearer header on every platform API call.\n  token_endpoint_path: /auth/m2m-token\n  token_request_params:\n  - client_id\n  - client_secret\n  response_field: access_token\n  header: 'Authorization: Bearer <token>'\n  sources:\n  - https://uniphore.github.io/baic-docs/\n- name: oidcSso\n  type: openIdConnect\n  description: >-\n    BAIC deployments\
  \ support enterprise OIDC single sign-on, configured through\n    the forge-user-management service (oidcSso.oauthBaseUrl) and an oidc-secrets\n    Kubernetes Secret. The identity provider is customer-supplied.\n  configurable: true\n  sources:\n  - https://uniphore.github.io/baic-docs/\nx-evidence:\n- url: https://uniphore.us.auth0.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-02'\n- url: https://uniphore.us.auth0.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-02'\n- url: https://uniphore.github.io/baic-docs/\n  http_status: 200\n  content_type: text/html\n  fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniphore/refs/heads/main/authentication/uniphore-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Company
- Artificial Intelligence
- Agents
- Conversational AI
- Customer Data Platform
- Contact Center
- Machine Learning
- Large Language Models
- Enterprise Software
- Automation
- Customer Experience
- Knowledge Management
---
