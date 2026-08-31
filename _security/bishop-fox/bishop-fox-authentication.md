---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bishop Fox Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bishop Fox secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bishop Fox
provider_slug: bishop-fox
scheme_count: 2
schemes:
- audience: cosmos_public
  credentials:
    client_id: Cosmos API key
    client_secret: Cosmos API secret
    issued_from: Cosmos portal (https://cosmos.bishopfox.com/)
  flow: clientCredentials
  name: CosmosOAuth2ClientCredentials
  scopes_documented: scopes/bishop-fox-scopes.yml
  source: https://docs.brinqa.com/docs/connectors/bishopfox/
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  token_lifetime_seconds: 36000
  token_url: https://bishopfox.auth0.com/oauth/token
  type: oauth2
- bearer_format: JWT
  description: 'The access token returned by the Auth0 client-credentials exchange is sent on every Cosmos v5 request as Authorization: Bearer <token>.'
  in: header
  name: CosmosBearerToken
  parameter_name: Authorization
  scheme: bearer
  source: https://docs.brinqa.com/docs/connectors/bishopfox/
  type: http
slug: bishop-fox-authentication
source_filename: bishop-fox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://bishopfox.auth0.com/.well-known/openid-configuration\ndocs: https://docs.brinqa.com/docs/connectors/bishopfox/\nnote: >-\n  Bishop Fox publishes no OpenAPI for the Cosmos v5 API and its reference documentation sits behind the\n  authenticated Cosmos portal, so this profile is NOT derived from a spec. It is assembled from two evidenced\n  sources: the anonymous OIDC/RFC 8414 discovery documents served by the Bishop Fox Auth0 tenant (harvested\n  verbatim to well-known/), and the published third-party connector documentation for Cosmos (Brinqa,\n  Axonius). Live probes of api.cosmos.bishopfox.com confirm the API is reachable and rejects anonymous\n  requests with HTTP 401.\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  bearer_format: JWT\n  anonymous_access: false\nschemes:\n- name: CosmosOAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url:\
  \ https://bishopfox.auth0.com/oauth/token\n  audience: cosmos_public\n  credentials:\n    client_id: Cosmos API key\n    client_secret: Cosmos API secret\n    issued_from: Cosmos portal (https://cosmos.bishopfox.com/)\n  token_lifetime_seconds: 36000\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  scopes_documented: scopes/bishop-fox-scopes.yml\n  source: https://docs.brinqa.com/docs/connectors/bishopfox/\n- name: CosmosBearerToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  parameter_name: Authorization\n  description: >-\n    The access token returned by the Auth0 client-credentials exchange is sent on every Cosmos v5 request as\n    Authorization: Bearer <token>.\n  source: https://docs.brinqa.com/docs/connectors/bishopfox/\nauthorization_server:\n  issuer: https://bishopfox.auth0.com/\n  vendor: Auth0\n  discovery:\n  - path: /.well-known/openid-configuration\n    file: ../well-known/bishop-fox-openid-configuration.json\n\
  \    http_status: 200\n  - path: /.well-known/oauth-authorization-server\n    file: ../well-known/bishop-fox-oauth-authorization-server.json\n    http_status: 200\n  authorization_endpoint: https://bishopfox.auth0.com/authorize\n  token_endpoint: https://bishopfox.auth0.com/oauth/token\n  revocation_endpoint: https://bishopfox.auth0.com/oauth/revoke\n  device_authorization_endpoint: https://bishopfox.auth0.com/oauth/device/code\n  jwks_uri: https://bishopfox.auth0.com/.well-known/jwks.json\n  userinfo_endpoint: https://bishopfox.auth0.com/userinfo\n  registration_endpoint: https://bishopfox.auth0.com/oidc/register\n  mfa_challenge_endpoint: https://bishopfox.auth0.com/mfa/challenge\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported:\n\
  \  - S256\n  - plain\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  backchannel_logout_supported: true\nx-evidence:\n- url: https://bishopfox.auth0.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-02'\n- url: https://bishopfox.auth0.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-02'\n- url: https://api.cosmos.bishopfox.com/v5/findings\n  http_status: 401\n  body: '{\"message\":\"Unauthorized\"}'\n  fetched: '2026-08-02'\n- url: https://docs.brinqa.com/docs/connectors/bishopfox/\n  http_status: 200\n  kind: third-party connector documentation\n  fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bishop-fox/refs/heads/main/authentication/bishop-fox-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Cybersecurity
- offensive-security
- penetration-testing
- attack-surface-management
- exposure-management
- red-teaming
- vulnerability-management
- security-findings
- asset-discovery
- continuous-threat-exposure-management
- Authentication
---
