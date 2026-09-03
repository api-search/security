---
api_key_in:
- header
auth_types:
- apiKey
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Angellist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AngelList secures its APIs with apiKey, openIdConnect, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AngelList
provider_slug: angellist
scheme_count: 3
schemes:
- applies_to: AngelList Investor Management API (GraphQL)
  endpoint: https://portal-api.angellist.com/beta
  in: header
  key_prefixes:
  - endpoint: https://portal-api.angellist.com/beta
    environment: production
    prefix: sk_live
  - endpoint: https://portal-api-staging.angellist.com/beta
    environment: staging
    prefix: sk_test
  name: AngelListApiKey
  provisioning: API keys are issued by AngelList on request — email portal@angellist.com for API setup. There is no self-service key page.
  sources:
  - https://docs.angellist.com/docs/overview
  type: apiKey
- applies_to: venture.angellist.com, portal.angellist.com (web sign-in)
  authorization_endpoint: https://auth.angellist.com/authorize
  claims_supported:
  - sub
  - iss
  - aud
  - exp
  - iat
  - auth_time
  - nonce
  - acr
  - amr
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://auth.angellist.com/end-session
  grant_types_supported:
  - authorization_code
  - refresh_token
  id_token_signing_alg_values_supported:
  - EdDSA
  issuer: https://auth.angellist.com
  jwks_uri: https://auth.angellist.com/.well-known/jwks.json
  name: AngelListOIDC
  openIdConnectUrl: https://auth.angellist.com/.well-known/openid-configuration
  registration_endpoint: https://auth.angellist.com/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://auth.angellist.com/token/revoke
  sources:
  - well-known/angellist-auth-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://auth.angellist.com/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
  type: openIdConnect
- applies_to: The documentation MCP surface advertised by https://docs.angellist.com/.well-known/oauth-protected-resource. The MCP endpoint itself currently answers 403 "MCP auth is not enabled for this deployment" — see mcp/angellist-mcp.yml.
  authorization_endpoint: https://docs.angellist.com/mcp/oauth/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://docs.angellist.com/mcp/oauth
  name: AngelListDocsMCPOAuth
  registration_endpoint: https://docs.angellist.com/mcp/oauth/register
  scopes_supported:
  - mcp:search
  sources:
  - well-known/angellist-docs-oauth-authorization-server.json
  - well-known/angellist-docs-oauth-protected-resource.json
  status: advertised
  token_endpoint: https://docs.angellist.com/mcp/oauth/token
  type: oauth2
slug: angellist-authentication
source_filename: angellist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://auth.angellist.com/.well-known/openid-configuration (probed) +\n  https://docs.angellist.com/docs/overview (API key model; docs host now\n  requires a login, values read from its publicly indexed copy)\ndocs: https://docs.angellist.com/docs/overview\nnote: >-\n  AngelList runs two distinct authentication models. The Investor Management\n  GraphQL API is a bearer API-key API with environment-scoped key prefixes. The\n  AngelList web products (venture.angellist.com, portal.angellist.com) sit\n  behind a first-party OIDC provider at auth.angellist.com that publishes real\n  RFC 8414 / OIDC discovery metadata and supports dynamic client registration.\n  No OpenAPI exists to derive securitySchemes from — the API is GraphQL and its\n  production endpoint has introspection disabled.\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  pkce:\
  \ S256\n  dynamic_client_registration: true\nschemes:\n- name: AngelListApiKey\n  type: apiKey\n  in: header\n  applies_to: AngelList Investor Management API (GraphQL)\n  endpoint: https://portal-api.angellist.com/beta\n  key_prefixes:\n  - prefix: sk_live\n    environment: production\n    endpoint: https://portal-api.angellist.com/beta\n  - prefix: sk_test\n    environment: staging\n    endpoint: https://portal-api-staging.angellist.com/beta\n  provisioning: >-\n    API keys are issued by AngelList on request — email portal@angellist.com for\n    API setup. There is no self-service key page.\n  sources:\n  - https://docs.angellist.com/docs/overview\n- name: AngelListOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.angellist.com/.well-known/openid-configuration\n  issuer: https://auth.angellist.com\n  authorization_endpoint: https://auth.angellist.com/authorize\n  token_endpoint: https://auth.angellist.com/token\n  revocation_endpoint: https://auth.angellist.com/token/revoke\n\
  \  end_session_endpoint: https://auth.angellist.com/end-session\n  jwks_uri: https://auth.angellist.com/.well-known/jwks.json\n  registration_endpoint: https://auth.angellist.com/oauth/register\n  id_token_signing_alg_values_supported:\n  - EdDSA\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - none\n  subject_types_supported:\n  - public\n  claims_supported:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - auth_time\n  - nonce\n  - acr\n  - amr\n  applies_to: venture.angellist.com, portal.angellist.com (web sign-in)\n  sources:\n  - well-known/angellist-auth-openid-configuration.json\n- name: AngelListDocsMCPOAuth\n  type: oauth2\n  status: advertised\n  issuer: https://docs.angellist.com/mcp/oauth\n  authorization_endpoint: https://docs.angellist.com/mcp/oauth/authorize\n  token_endpoint: https://docs.angellist.com/mcp/oauth/token\n\
  \  registration_endpoint: https://docs.angellist.com/mcp/oauth/register\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  scopes_supported:\n  - mcp:search\n  applies_to: >-\n    The documentation MCP surface advertised by\n    https://docs.angellist.com/.well-known/oauth-protected-resource. The MCP\n    endpoint itself currently answers 403 \"MCP auth is not enabled for this\n    deployment\" — see mcp/angellist-mcp.yml.\n  sources:\n  - well-known/angellist-docs-oauth-authorization-server.json\n  - well-known/angellist-docs-oauth-protected-resource.json\nprotected_resource_metadata:\n- resource: https://docs.angellist.com\n  authorization_servers:\n  - https://docs.angellist.com/mcp/oauth\n  source: well-known/angellist-docs-oauth-protected-resource.json\n  rfc: RFC 9728\nx-evidence:\n- url: https://auth.angellist.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n\
  - url: https://auth.angellist.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- url: https://docs.angellist.com/.well-known/oauth-protected-resource\n  http_status: 200\n  content_type: application/json\n- url: https://docs.angellist.com/docs/overview\n  http_status: 200\n  note: 302s to /login?redirect=%2Fdocs%2Foverview — auth-gated as of 2026-09-02\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angellist/refs/heads/main/authentication/angellist-authentication.yml
summary_line: apiKey/openIdConnect/oauth2 · 3 schemes
tags:
- Documents
- Funds
- Investing
- Job
- Startups
- Transaction
- Venture Capital
---
