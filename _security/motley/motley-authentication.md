---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: Motley Cloud's API and hosted MCP server (https://app.motley.ai/api/v1/) authenticate with OAuth 2.0 (RFC 8414 authorization server metadata, backed by Clerk), authorization-code flow with PKCE and OpenID Connect. The open-source SLayer server run locally holds database credentials itself and does not expose them to consumers.
kind: authentication
layout: security
method: searched
name: Motley Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Motley secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Motley
provider_slug: motley
scheme_count: 2
schemes:
- authorizationUrl: https://clerk.motley.ai/oauth/authorize
  flow: authorizationCode
  id_token_signing_alg:
  - RS256
  issuer: https://app.motley.ai
  jwks_uri: https://clerk.motley.ai/.well-known/jwks.json
  name: OAuth2
  registrationUrl: https://app.motley.ai/api/v1/oauth/register
  revocationUrl: https://clerk.motley.ai/oauth/token/revoke
  scopes_url: scopes/motley-scopes.yml
  sources:
  - well-known/motley-oauth-authorization-server.json
  tokenUrl: https://clerk.motley.ai/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- issuer: https://app.motley.ai
  name: OpenIDConnect
  note: OIDC claims include sub, iss, aud, exp, iat, email, name, org_id.
  sources:
  - well-known/motley-oauth-authorization-server.json
  type: openIdConnect
slug: motley-authentication
source_filename: motley-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.motley.ai/.well-known/oauth-authorization-server\ndocs: https://docs.motley.ai/slayer/getting-started/rest-api\ndescription: >-\n  Motley Cloud's API and hosted MCP server (https://app.motley.ai/api/v1/)\n  authenticate with OAuth 2.0 (RFC 8414 authorization server metadata, backed by\n  Clerk), authorization-code flow with PKCE and OpenID Connect. The open-source\n  SLayer server run locally holds database credentials itself and does not expose\n  them to consumers.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  oidc: true\n  pkce: [S256]\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://app.motley.ai\n  authorizationUrl: https://clerk.motley.ai/oauth/authorize\n  tokenUrl: https://clerk.motley.ai/oauth/token\n  revocationUrl: https://clerk.motley.ai/oauth/token/revoke\n  registrationUrl: https://app.motley.ai/api/v1/oauth/register\n\
  \  jwks_uri: https://clerk.motley.ai/.well-known/jwks.json\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  id_token_signing_alg: [RS256]\n  scopes_url: scopes/motley-scopes.yml\n  sources: [well-known/motley-oauth-authorization-server.json]\n- name: OpenIDConnect\n  type: openIdConnect\n  issuer: https://app.motley.ai\n  note: OIDC claims include sub, iss, aud, exp, iat, email, name, org_id.\n  sources: [well-known/motley-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motley/refs/heads/main/authentication/motley-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Semantic Layer
- Business Intelligence
- Analytics
- AI Agents
- MCP
- SQL
- Data
- Reporting
---
