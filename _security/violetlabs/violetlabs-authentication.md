---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: Violet Labs exposes two authentication models. The REST Explore API uses an API-key credential passed in an HTTP header. The hosted MCP server (and the broader app.violetlabs.com surface) additionally supports OAuth 2.0 with PKCE and dynamic client registration. API keys are created in Company Settings and may be given an optional expiration date.
kind: authentication
layout: security
method: searched
name: Violetlabs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Violetlabs secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Violetlabs
provider_slug: violetlabs
scheme_count: 2
schemes:
- applies_to: Violet Explore API (POST /api/explore) and API-key MCP clients.
  description: Tenant API key created in Company Settings > API Keys, passed on every REST request in the x-api-key header (the MCP server accepts the same key as X-API-Key). Keys can carry an optional expiration date.
  docs: https://docs.violetlabs.com/features/api/generate-an-api-key
  in: header
  name: apiKeyAuth
  parameter_name: x-api-key
  type: apiKey
- authorizationUrl: https://app.violetlabs.com/api/oauth/authorize
  description: OAuth 2.0 authorization server for the hosted MCP server. Users authenticate with existing Violet credentials and select a workspace. Supports PKCE (S256) and dynamic client registration (RFC 7591).
  discovery: well-known/violetlabs-openid-configuration.json
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  name: oauth2
  pkce: S256
  registrationUrl: https://app.violetlabs.com/api/oauth/register
  scopes:
    mcp: Access the Violet MCP server for the selected workspace.
  tokenUrl: https://app.violetlabs.com/api/oauth/token
  type: oauth2
slug: violetlabs-authentication
source_filename: violetlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://docs.violetlabs.com/features/api/generate-an-api-key,\n  https://docs.violetlabs.com/features/api/endpoints,\n  https://docs.violetlabs.com/ai/mcp, and the OAuth/OIDC discovery documents at\n  https://app.violetlabs.com/.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server.\ndocs: https://docs.violetlabs.com/features/api/generate-an-api-key\ndescription: >-\n  Violet Labs exposes two authentication models. The REST Explore API uses an\n  API-key credential passed in an HTTP header. The hosted MCP server (and the\n  broader app.violetlabs.com surface) additionally supports OAuth 2.0 with PKCE\n  and dynamic client registration. API keys are created in Company Settings and\n  may be given an optional expiration date.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter_name: x-api-key\n  description: >-\n    Tenant API key created in Company Settings > API Keys, passed on every REST\n    request in the x-api-key header (the MCP server accepts the same key as\n    X-API-Key). Keys can carry an optional expiration date.\n  applies_to: Violet Explore API (POST /api/explore) and API-key MCP clients.\n  docs: https://docs.violetlabs.com/features/api/generate-an-api-key\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization server for the hosted MCP server. Users authenticate\n    with existing Violet credentials and select a workspace. Supports PKCE\n    (S256) and dynamic client registration (RFC 7591).\n  authorizationUrl: https://app.violetlabs.com/api/oauth/authorize\n  tokenUrl: https://app.violetlabs.com/api/oauth/token\n  registrationUrl: https://app.violetlabs.com/api/oauth/register\n  grant_types: [authorization_code, refresh_token, client_credentials]\n  pkce: S256\n  scopes:\n    mcp: Access the\
  \ Violet MCP server for the selected workspace.\n  discovery: well-known/violetlabs-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/violetlabs/refs/heads/main/authentication/violetlabs-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Hardware
- Engineering
- Manufacturing
- PLM
- ERP
- Data Integration
- Requirements Management
- Aerospace
- Defense
- MCP
- Systems Engineering
---
