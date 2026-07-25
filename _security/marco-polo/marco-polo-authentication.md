---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Marco Polo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marco Polo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Marco Polo
provider_slug: marco-polo
scheme_count: 1
schemes:
- authorization_endpoint: https://appealing-lion-77-staging.authkit.app/oauth2/authorize
  authorization_server: https://appealing-lion-77-staging.authkit.app
  code_challenge_methods:
  - S256
  device_authorization_endpoint: https://appealing-lion-77-staging.authkit.app/oauth2/device_authorization
  dynamic_client_registration: supported (RFC 7591 registration_endpoint + client_id metadata documents)
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  identity_providers:
  - Google
  - Microsoft
  - GitHub
  - Email
  issuer: https://appealing-lion-77-staging.authkit.app
  jwks_uri: https://appealing-lion-77-staging.authkit.app/oauth2/jwks
  metadata_standards:
  - RFC 8414 (Authorization Server Metadata)
  - RFC 9728 (Protected Resource Metadata)
  name: oauth2
  registration_endpoint: https://appealing-lion-77-staging.authkit.app/oauth2/register
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  token_delivery: bearer (Authorization header)
  token_endpoint: https://appealing-lion-77-staging.authkit.app/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: marco-polo-authentication
source_filename: marco-polo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.marcopolo.dev/.well-known/oauth-authorization-server + https://docs.marcopolo.dev/getting-started\nprovider: marco-polo\nsummary: >-\n  MarcoPolo authenticates MCP clients with OAuth 2.0 (authorization-code + PKCE,\n  plus a device-authorization grant), fronted by WorkOS AuthKit. End users sign\n  in with Google, Microsoft, GitHub, or email; the issued bearer token is sent in\n  the Authorization header to the protected MCP resource at https://mcp.marcopolo.dev.\ndocs: https://docs.marcopolo.dev/getting-started\nschemes:\n- name: oauth2\n  type: oauth2\n  authorization_server: https://appealing-lion-77-staging.authkit.app\n  authorization_endpoint: https://appealing-lion-77-staging.authkit.app/oauth2/authorize\n  device_authorization_endpoint: https://appealing-lion-77-staging.authkit.app/oauth2/device_authorization\n  token_endpoint: https://appealing-lion-77-staging.authkit.app/oauth2/token\n  registration_endpoint:\
  \ https://appealing-lion-77-staging.authkit.app/oauth2/register\n  jwks_uri: https://appealing-lion-77-staging.authkit.app/oauth2/jwks\n  issuer: https://appealing-lion-77-staging.authkit.app\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - offline_access\n  code_challenge_methods:\n  - S256\n  token_delivery: bearer (Authorization header)\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  dynamic_client_registration: 'supported (RFC 7591 registration_endpoint + client_id metadata documents)'\n  metadata_standards:\n  - RFC 8414 (Authorization Server Metadata)\n  - RFC 9728 (Protected Resource Metadata)\n  identity_providers:\n  - Google\n  - Microsoft\n  - GitHub\n  - Email\nidentity_mapping: >-\n  Domain-based identity mapping connects users to their company environment for\n  shared workspace resources.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marco-polo/refs/heads/main/authentication/marco-polo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- MCP
- Model Context Protocol
- Enterprise AI
- Data Governance
- AI Agents
- Data Integration
- Security
- OAuth
---
