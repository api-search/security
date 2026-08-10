---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Uptake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uptake declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Uptake
provider_slug: uptake
scheme_count: 3
schemes:
- dynamic_client_registration: true
  endpoints:
    authorization: https://start.uptake.com/oauth2/v1/authorize
    introspection: https://start.uptake.com/oauth2/v1/introspect
    jwks: https://start.uptake.com/oauth2/v1/keys
    registration: https://start.uptake.com/oauth2/v1/clients
    revocation: https://start.uptake.com/oauth2/v1/revoke
    token: https://start.uptake.com/oauth2/v1/token
    userinfo: https://start.uptake.com/oauth2/v1/userinfo
  evidence:
    content_type: application/json
    fetched: '2026-08-05'
    file: well-known/uptake-openid-configuration.json
    http_status: 200
    url: https://start.uptake.com/.well-known/openid-configuration
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  id: uptake-oidc
  id_token_signing_alg_values_supported:
  - RS256
  identity_provider: Okta (custom domain)
  in: null
  issuer: https://start.uptake.com
  openIdConnectUrl: https://start.uptake.com/.well-known/openid-configuration
  pkce: true
  pkce_code_challenge_methods:
  - S256
  response_types_supported:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  scheme: null
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- evidence:
    content_type: application/json
    fetched: '2026-08-05'
    file: well-known/uptake-oauth-authorization-server.json
    http_status: 200
    url: https://start.uptake.com/.well-known/oauth-authorization-server
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  id: uptake-oauth-authorization-server
  issuer: https://start.uptake.com
  metadata: RFC 8414
  metadata_url: https://start.uptake.com/.well-known/oauth-authorization-server
  note: Adds client_credentials over the OIDC document. The scopes_supported list on this document is Okta's own org-management scope set (okta.*), exposed because the tenant fronts the Okta management API — it is not the Uptake product API scope set. See scopes/uptake-scopes.yml.
  type: oauth2
- companion_headers:
  - Authorization (Bearer)
  - Tenant
  confidence: medium
  evidence:
    fetched: '2026-08-05'
    http_status: 200
    url: https://www.cozyroc.com/ssis/uptake-cloudlink-connection
  first_party_documented: false
  id: uptake-platform-api-key
  in: header
  name: x-api-key
  note: NOT confirmed against an Uptake-published document. Reconstructed from a third-party connector reference (COZYROC "Uptake CloudLink Connection", base https://use-api.cloudlink.uptake.com/v1/), which describes session-token auth with a required Tenant and apiKey and the three headers above. The cloudlink.uptake.com hostname no longer resolves in DNS, so the CloudLink product surface appears retired; the current gateway at api.uptake.com was not confirmed to use the same scheme.
  type: apiKey
slug: uptake-authentication
source_filename: uptake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://start.uptake.com/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  Uptake has no published OpenAPI, so this profile is built from what the estate\n  actually serves. Two authentication models are visible from outside. (1) Human\n  and application sign-in to the Uptake platform is OpenID Connect against an Okta\n  tenant on Uptake's own custom domain, start.uptake.com — the discovery document\n  is public and is saved verbatim under well-known/. (2) The machine API surface\n  at api.uptake.com and api.common.uptake.com is an AWS API Gateway that returns\n  403 ForbiddenException to every anonymous request; third-party integration\n  documentation (COZYROC's Uptake CloudLink connector) describes that surface as\n  key-based, sending a tenant header, a bearer Authorization header and an\n  x-api-key header. Key issuance is not self-service: Fleetio's integration guide\n  instructs customers to send their token\
  \ to an Uptake account representative who\n  completes the connection.\nschemes:\n- id: uptake-oidc\n  type: openIdConnect\n  in: null\n  scheme: null\n  openIdConnectUrl: https://start.uptake.com/.well-known/openid-configuration\n  issuer: https://start.uptake.com\n  identity_provider: Okta (custom domain)\n  endpoints:\n    authorization: https://start.uptake.com/oauth2/v1/authorize\n    token: https://start.uptake.com/oauth2/v1/token\n    userinfo: https://start.uptake.com/oauth2/v1/userinfo\n    jwks: https://start.uptake.com/oauth2/v1/keys\n    registration: https://start.uptake.com/oauth2/v1/clients\n    revocation: https://start.uptake.com/oauth2/v1/revoke\n    introspection: https://start.uptake.com/oauth2/v1/introspect\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types_supported:\n  - code\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code\
  \ id_token token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values_supported:\n  - RS256\n  pkce: true\n  pkce_code_challenge_methods:\n  - S256\n  dynamic_client_registration: true\n  evidence:\n    url: https://start.uptake.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n    fetched: '2026-08-05'\n    file: well-known/uptake-openid-configuration.json\n- id: uptake-oauth-authorization-server\n  type: oauth2\n  metadata: RFC 8414\n  metadata_url: https://start.uptake.com/.well-known/oauth-authorization-server\n  issuer: https://start.uptake.com\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  note: >-\n    Adds client_credentials over the OIDC document. The scopes_supported list on\n    this\
  \ document is Okta's own org-management scope set (okta.*), exposed\n    because the tenant fronts the Okta management API — it is not the Uptake\n    product API scope set. See scopes/uptake-scopes.yml.\n  evidence:\n    url: https://start.uptake.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n    fetched: '2026-08-05'\n    file: well-known/uptake-oauth-authorization-server.json\n- id: uptake-platform-api-key\n  type: apiKey\n  in: header\n  name: x-api-key\n  companion_headers:\n  - Authorization (Bearer)\n  - Tenant\n  confidence: medium\n  first_party_documented: false\n  note: >-\n    NOT confirmed against an Uptake-published document. Reconstructed from a\n    third-party connector reference (COZYROC \"Uptake CloudLink Connection\",\n    base https://use-api.cloudlink.uptake.com/v1/), which describes session-token\n    auth with a required Tenant and apiKey and the three headers above. The\n    cloudlink.uptake.com hostname no\
  \ longer resolves in DNS, so the CloudLink\n    product surface appears retired; the current gateway at api.uptake.com was\n    not confirmed to use the same scheme.\n  evidence:\n    url: https://www.cozyroc.com/ssis/uptake-cloudlink-connection\n    http_status: 200\n    fetched: '2026-08-05'\ngated_surfaces:\n- url: https://api.uptake.com/\n  http_status: 403\n  body: '{\"message\":\"Forbidden\"}'\n  note: AWS API Gateway ForbiddenException; no WWW-Authenticate challenge is returned, so no scheme is advertised anonymously.\n- url: https://api.common.uptake.com/\n  http_status: 403\n  note: Same behavior.\n- url: https://developer.uptake.com/\n  http_status: 404\n  note: Former developer portal, now dead.\nchecked: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptake/refs/heads/main/authentication/uptake-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Industrial AI
- Predictive Maintenance
- Asset Performance Management
- Fleet Management
- Telematics
- Machine Learning
- Industrial IoT
---
