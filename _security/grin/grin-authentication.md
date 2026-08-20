---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Grin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- tokenExchange
overview: Grin secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, and tokenExchange flow(s).
provider_name: Grin
provider_slug: grin
scheme_count: 2
schemes:
- authorizationUrl: https://auth.grin.co/authorize
  code_challenge_methods:
  - S256
  - plain
  deviceAuthorizationEndpoint: https://auth.grin.co/oauth/device/code
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://auth.grin.co/
  jwksUri: https://auth.grin.co/.well-known/jwks.json
  name: GrinOIDC
  openIdConnectUrl: https://auth.grin.co/.well-known/openid-configuration
  provider: Auth0 (GRIN-operated tenant on auth.grin.co)
  registrationEndpoint: https://auth.grin.co/oidc/register
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/grin-openid-configuration.json
  - well-known/grin-oauth-authorization-server.json
  tokenUrl: https://auth.grin.co/oauth/token
  type: openIdConnect
  userinfoUrl: https://auth.grin.co/userinfo
- applies_to: https://mcp.grin.co/mcp
  authorization_servers:
  - https://auth.grin.co/
  bearer_methods_supported:
  - header
  challenge: 'WWW-Authenticate: Bearer resource_metadata="https://mcp.grin.co/.well-known/oauth-protected-resource"'
  name: GrinMCPBearer
  scheme: Bearer token in the Authorization header
  scopes:
  - openid
  - email
  - profile
  sources:
  - well-known/grin-oauth-protected-resource.json
  standard: RFC 9728 OAuth 2.0 Protected Resource Metadata
  type: oauth2
slug: grin-authentication
source_filename: grin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.grin.co/.well-known/openid-configuration\ndocs: https://grin.co/security/\nnote: >-\n  No OpenAPI is publicly reachable for GRIN (see lifecycle/grin-lifecycle.yml —\n  the Stoplight documentation project GRIN links from its own docs host returns\n  404), so this profile is NOT derived from securitySchemes. It is probed\n  directly from the two anonymous discovery documents GRIN's own hosts serve:\n  the OIDC/RFC 8414 metadata on auth.grin.co (an Auth0 tenant on GRIN's domain)\n  and the RFC 9728 protected-resource metadata on mcp.grin.co. Those describe\n  the auth model in front of the GRIN app and the Gia MCP server. The\n  authentication model for the legacy read-only REST API described on the\n  Stoplight workspace home (\"uses standard HTTP response codes and\n  authentication\") is NOT publicly documented and is deliberately not guessed\n  here.\n\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in:\
  \ []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  - deviceCode\n  - tokenExchange\n  pkce: true\n  dynamic_client_registration: true\n\nschemes:\n- name: GrinOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.grin.co/.well-known/openid-configuration\n  issuer: https://auth.grin.co/\n  provider: Auth0 (GRIN-operated tenant on auth.grin.co)\n  authorizationUrl: https://auth.grin.co/authorize\n  tokenUrl: https://auth.grin.co/oauth/token\n  userinfoUrl: https://auth.grin.co/userinfo\n  jwksUri: https://auth.grin.co/.well-known/jwks.json\n  registrationEndpoint: https://auth.grin.co/oidc/register\n  deviceAuthorizationEndpoint: https://auth.grin.co/oauth/device/code\n  code_challenge_methods:\n  - S256\n  - plain\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n\
  \  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  sources:\n  - well-known/grin-openid-configuration.json\n  - well-known/grin-oauth-authorization-server.json\n\n- name: GrinMCPBearer\n  type: oauth2\n  applies_to: https://mcp.grin.co/mcp\n  scheme: Bearer token in the Authorization header\n  bearer_methods_supported:\n  - header\n  authorization_servers:\n  - https://auth.grin.co/\n  scopes:\n  - openid\n  - email\n  - profile\n  challenge: >-\n    WWW-Authenticate: Bearer resource_metadata=\"https://mcp.grin.co/.well-known/oauth-protected-resource\"\n  standard: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  sources:\n  - well-known/grin-oauth-protected-resource.json\n\napp_login:\n  url: https://app.grin.co/login\n  flow: >-\n    app.grin.co 302s to https://auth.grin.co/authorize with response_type=code,\n    scope=\"openid profile email\" and prompt=select_account\
  \ — an authorization\n    code flow against the same tenant that fronts the MCP server.\n  observed_status: 302\n\nx-evidence:\n- url: https://auth.grin.co/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://auth.grin.co/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://mcp.grin.co/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://app.grin.co/\n  http_status: 302\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grin/refs/heads/main/authentication/grin-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Influencer Marketing
- Creator Economy
- Creator Management
- Affiliate Marketing
- Marketing
- Social-Media
- E-Commerce
---
