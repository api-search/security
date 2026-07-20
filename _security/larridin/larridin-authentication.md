---
api_key_in:
- header
api_specs:
- filename: larridin-scout-openapi.yml
  format: yaml
  label: Larridin Scout API v1
  slug: scout-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/larridin/refs/heads/main/openapi/larridin-scout-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Larridin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- deviceCode
overview: Larridin secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and deviceCode flow(s).
provider_name: Larridin
provider_slug: larridin
scheme_count: 2
schemes:
- applies_to: Scout API v1 (https://scout-api.larridin.com/api/v1)
  description: Company API key. The ANALYTICS scope is required for Scout API v1 endpoints.
  docs: https://docs.larridin.com/api/scout-api-v1-reference
  in: header
  name: companyApiKey
  parameter: x-company-api-key
  sources:
  - openapi/larridin-scout-openapi.yml
  type: apiKey
- applies_to: Larridin MCP server (https://app.larridin.com/mcp/larridin)
  authorization_endpoint: https://login.larridin.com/oauth2/authorize
  bearer_methods_supported:
  - header
  description: OAuth 2.0 authorization used by the Larridin MCP server. Compatible MCP clients discover the authorization-server and protected-resource metadata and prompt the user to sign in.
  device_authorization_endpoint: https://login.larridin.com/oauth2/device_authorization
  docs: https://docs.larridin.com/api/mcp
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://login.larridin.com/oauth2/introspection
  issuer: https://login.larridin.com
  jwks_uri: https://login.larridin.com/oauth2/jwks
  name: larridinOAuth
  pkce_methods:
  - S256
  registration_endpoint: https://login.larridin.com/oauth2/register
  sources:
  - well-known/larridin-oauth-authorization-server.json
  - well-known/larridin-oauth-protected-resource.json
  token_endpoint: https://login.larridin.com/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: larridin-authentication
source_filename: larridin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/larridin-scout-openapi.yml\ndocs: https://docs.larridin.com/api/scout-api-v1-reference\nnotes: >-\n  Larridin runs two distinct authentication models. The Scout REST API v1 uses a company API key in the\n  x-company-api-key header and requires the ANALYTICS scope. The beta MCP server at /mcp/larridin uses\n  OAuth 2.0 with an authorization server at https://login.larridin.com, discovered via RFC 8414\n  authorization-server metadata and RFC 9728 protected-resource metadata. End-user access to the\n  Larridin application itself is documented as SSO.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - deviceCode\nschemes:\n- name: companyApiKey\n  type: apiKey\n  in: header\n  parameter: x-company-api-key\n  description: Company API key. The ANALYTICS scope is required for Scout API v1 endpoints.\n  applies_to: Scout API v1 (https://scout-api.larridin.com/api/v1)\n\
  \  docs: https://docs.larridin.com/api/scout-api-v1-reference\n  sources:\n  - openapi/larridin-scout-openapi.yml\n- name: larridinOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization used by the Larridin MCP server. Compatible MCP clients discover the\n    authorization-server and protected-resource metadata and prompt the user to sign in.\n  applies_to: Larridin MCP server (https://app.larridin.com/mcp/larridin)\n  issuer: https://login.larridin.com\n  authorization_endpoint: https://login.larridin.com/oauth2/authorize\n  token_endpoint: https://login.larridin.com/oauth2/token\n  jwks_uri: https://login.larridin.com/oauth2/jwks\n  registration_endpoint: https://login.larridin.com/oauth2/register\n  introspection_endpoint: https://login.larridin.com/oauth2/introspection\n  device_authorization_endpoint: https://login.larridin.com/oauth2/device_authorization\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n\
  \  pkce_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  dynamic_client_registration: true\n  bearer_methods_supported:\n  - header\n  docs: https://docs.larridin.com/api/mcp\n  sources:\n  - well-known/larridin-oauth-authorization-server.json\n  - well-known/larridin-oauth-protected-resource.json\nsso:\n  documented: true\n  docs: https://docs.larridin.com/setup/sso\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/larridin/refs/heads/main/authentication/larridin-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Adoption
- AI Governance
- Analytics
- Developer Productivity
- Developer Intelligence
- Workflow Intelligence
- Enterprise Software
- Observability
---
