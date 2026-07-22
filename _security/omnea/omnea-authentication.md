---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: Omnea's remote MCP surface (mcp.omnea.co) is protected by OAuth 2.0 / OpenID Connect, with the authorization server delegated to WorkOS AuthKit (https://personal-flight-18.authkit.app). Discovery documents advertise authorization-code (with PKCE S256), client-credentials, device-code and refresh-token grants, dynamic client registration (RFC 7591), and a public bearer-token protected resource per RFC 9728. The Omnea public REST API (app.omnea.co/public-api) is documented but its scheme was not enumerable unauthenticated.
kind: authentication
layout: security
method: searched
name: Omnea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Omnea secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Omnea
provider_slug: omnea
scheme_count: 1
schemes:
- authorization_endpoint: https://personal-flight-18.authkit.app/oauth2/authorize
  bearer_methods:
  - header
  code_challenge_methods:
  - S256
  description: OAuth 2.0 authorization for the Omnea remote MCP server, backed by WorkOS AuthKit. PKCE (S256) required for the authorization-code flow; dynamic client registration supported.
  device_authorization_endpoint: https://personal-flight-18.authkit.app/oauth2/device_authorization
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://personal-flight-18.authkit.app/oauth2/introspection
  issuer: https://personal-flight-18.authkit.app
  jwks_uri: https://personal-flight-18.authkit.app/oauth2/jwks
  name: oauth2
  protected_resource: https://mcp.omnea.co
  registration_endpoint: https://personal-flight-18.authkit.app/oauth2/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/omnea-mcp-oauth-authorization-server.json
  - well-known/omnea-mcp-openid-configuration.json
  - well-known/omnea-mcp-oauth-protected-resource.json
  token_endpoint: https://personal-flight-18.authkit.app/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://personal-flight-18.authkit.app/oauth2/userinfo
slug: omnea-authentication
source_filename: omnea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://mcp.omnea.co/.well-known/oauth-authorization-server,\n  https://mcp.omnea.co/.well-known/openid-configuration,\n  https://mcp.omnea.co/.well-known/oauth-protected-resource\ndescription: >-\n  Omnea's remote MCP surface (mcp.omnea.co) is protected by OAuth 2.0 / OpenID\n  Connect, with the authorization server delegated to WorkOS AuthKit\n  (https://personal-flight-18.authkit.app). Discovery documents advertise\n  authorization-code (with PKCE S256), client-credentials, device-code and\n  refresh-token grants, dynamic client registration (RFC 7591), and a public\n  bearer-token protected resource per RFC 9728. The Omnea public REST API\n  (app.omnea.co/public-api) is documented but its scheme was not enumerable\n  unauthenticated.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\nschemes:\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization for the Omnea remote MCP server, backed by\
  \ WorkOS\n    AuthKit. PKCE (S256) required for the authorization-code flow; dynamic\n    client registration supported.\n  issuer: https://personal-flight-18.authkit.app\n  authorization_endpoint: https://personal-flight-18.authkit.app/oauth2/authorize\n  token_endpoint: https://personal-flight-18.authkit.app/oauth2/token\n  registration_endpoint: https://personal-flight-18.authkit.app/oauth2/register\n  device_authorization_endpoint: https://personal-flight-18.authkit.app/oauth2/device_authorization\n  introspection_endpoint: https://personal-flight-18.authkit.app/oauth2/introspection\n  userinfo_endpoint: https://personal-flight-18.authkit.app/oauth2/userinfo\n  jwks_uri: https://personal-flight-18.authkit.app/oauth2/jwks\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n\
  \  - RS256\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  protected_resource: https://mcp.omnea.co\n  bearer_methods:\n  - header\n  sources:\n  - well-known/omnea-mcp-oauth-authorization-server.json\n  - well-known/omnea-mcp-openid-configuration.json\n  - well-known/omnea-mcp-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnea/refs/heads/main/authentication/omnea-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Ai
- Procurement
- Source-to-Pay
- Supplier Management
- Spend Management
- Agents
- MCP
---
