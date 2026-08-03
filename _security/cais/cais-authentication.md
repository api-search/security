---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: 'CAIS runs two distinct identity surfaces. (1) The MCP server at mcp.caisgroup.com is its own OAuth 2.1 authorization server: authorization-code + PKCE S256, refresh tokens, RFC 7591 dynamic client registration, RFC 7009 revocation, RFC 9728 protected-resource metadata, and bearer tokens in the Authorization header only. It supports client_id metadata documents. (2) The member platform behind members.caisgroup.com authenticates through an Auth0 tenant on the custom domain login.caisgroup.com, which publishes full OpenID Connect Discovery 1.0 metadata including MFA challenge and device-authorization endpoints. No API key, HTTP basic, or mutualTLS scheme is advertised on any public CAIS surface.'
kind: authentication
layout: security
method: probed
name: Cais Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CAIS secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CAIS
provider_slug: cais
scheme_count: 2
schemes:
- applies_to: https://mcp.caisgroup.com/mcp
  bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://mcp.caisgroup.com/authorize
    flow: authorizationCode
    registrationUrl: https://mcp.caisgroup.com/register
    revocationUrl: https://mcp.caisgroup.com/revoke
    scope_count: 12
    tokenUrl: https://mcp.caisgroup.com/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.caisgroup.com/
  name: cais-mcp-oauth
  protected_resource_metadata: well-known/cais-oauth-protected-resource.json
  response_types_supported:
  - code
  revocation_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  sources:
  - well-known/cais-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- applies_to: https://members.caisgroup.com
  authorizationUrl: https://login.caisgroup.com/authorize
  code_challenge_methods_supported:
  - S256
  - plain
  device_authorization_endpoint: https://login.caisgroup.com/oauth/device/code
  issuer: https://login.caisgroup.com/
  jwksUri: https://login.caisgroup.com/.well-known/jwks.json
  mfa_challenge_endpoint: https://login.caisgroup.com/mfa/challenge
  name: cais-members-oidc
  openIdConnectUrl: https://login.caisgroup.com/.well-known/openid-configuration
  provider: Auth0 (custom domain)
  registrationUrl: https://login.caisgroup.com/oidc/register
  revocationUrl: https://login.caisgroup.com/oauth/revoke
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  sources:
  - well-known/cais-openid-configuration.json
  tokenUrl: https://login.caisgroup.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfoUrl: https://login.caisgroup.com/userinfo
slug: cais-authentication
source_filename: cais-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: >-\n  https://mcp.caisgroup.com/.well-known/oauth-authorization-server,\n  https://mcp.caisgroup.com/.well-known/oauth-protected-resource,\n  https://login.caisgroup.com/.well-known/openid-configuration\ndescription: >-\n  CAIS runs two distinct identity surfaces. (1) The MCP server at mcp.caisgroup.com\n  is its own OAuth 2.1 authorization server: authorization-code + PKCE S256, refresh\n  tokens, RFC 7591 dynamic client registration, RFC 7009 revocation, RFC 9728\n  protected-resource metadata, and bearer tokens in the Authorization header only.\n  It supports client_id metadata documents. (2) The member platform behind\n  members.caisgroup.com authenticates through an Auth0 tenant on the custom domain\n  login.caisgroup.com, which publishes full OpenID Connect Discovery 1.0 metadata\n  including MFA challenge and device-authorization endpoints. No API key, HTTP basic,\n  or mutualTLS scheme is advertised on any public CAIS\
  \ surface.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_in: [header]\n  pkce: [S256]\n  dynamic_client_registration: true\n  mfa: true\nschemes:\n- name: cais-mcp-oauth\n  type: oauth2\n  applies_to: https://mcp.caisgroup.com/mcp\n  issuer: https://mcp.caisgroup.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.caisgroup.com/authorize\n    tokenUrl: https://mcp.caisgroup.com/token\n    revocationUrl: https://mcp.caisgroup.com/revoke\n    registrationUrl: https://mcp.caisgroup.com/register\n    scope_count: 12\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  revocation_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  client_id_metadata_document_supported: true\n  bearer_methods_supported: [header]\n\
  \  protected_resource_metadata: well-known/cais-oauth-protected-resource.json\n  sources: [well-known/cais-oauth-authorization-server.json]\n- name: cais-members-oidc\n  type: openIdConnect\n  applies_to: https://members.caisgroup.com\n  provider: Auth0 (custom domain)\n  issuer: https://login.caisgroup.com/\n  openIdConnectUrl: https://login.caisgroup.com/.well-known/openid-configuration\n  authorizationUrl: https://login.caisgroup.com/authorize\n  tokenUrl: https://login.caisgroup.com/oauth/token\n  userinfoUrl: https://login.caisgroup.com/userinfo\n  jwksUri: https://login.caisgroup.com/.well-known/jwks.json\n  registrationUrl: https://login.caisgroup.com/oidc/register\n  revocationUrl: https://login.caisgroup.com/oauth/revoke\n  device_authorization_endpoint: https://login.caisgroup.com/oauth/device/code\n  mfa_challenge_endpoint: https://login.caisgroup.com/mfa/challenge\n  scopes_supported: [openid, profile, offline_access, name, given_name, family_name,\n    nickname, email, email_verified,\
  \ picture, created_at, identities, phone, address]\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post,\n    private_key_jwt, none]\n  sources: [well-known/cais-openid-configuration.json]\nobservations:\n- >-\n  The MCP server's WWW-Authenticate challenge points resource_metadata at\n  https://mcp.caisgroup.com/.well-known/oauth-protected-resource/mcp, but that\n  suffixed path returns 404; the document is only reachable at the unsuffixed\n  /.well-known/oauth-protected-resource. A strictly conformant RFC 9728 client that\n  follows the advertised URL will fail to resolve the metadata.\n- >-\n  The MCP authorization server advertises no OIDC discovery document of its own\n  (/.well-known/openid-configuration returns 404) despite advertising the \"openid\"\n  scope.\ndocs: null\ndocs_note: CAIS publishes no public developer authentication documentation.\nx-evidence:\n  fetched: '2026-08-01'\n  probes:\n  -\
  \ {url: 'https://mcp.caisgroup.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://mcp.caisgroup.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://mcp.caisgroup.com/.well-known/oauth-protected-resource/mcp', http_status: 404}\n  - {url: 'https://login.caisgroup.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://login.caisgroup.com/.well-known/jwks.json', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cais/refs/heads/main/authentication/cais-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Alternative Investments
- Wealth Management
- Financial Services
- Fintech
- Private Markets
- Asset Management
- Structured Products
- Investment Platform
- Artificial Intelligence
---
