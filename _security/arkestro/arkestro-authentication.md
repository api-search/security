---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: arkestro-webhooks-api-openapi.yml
  format: yaml
  label: Arkestro Webhooks API
  slug: arkestro-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkestro/openapi/arkestro-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Arkestro Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Arkestro secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Arkestro
provider_slug: arkestro
scheme_count: 2
schemes:
- example_usage: 'curl --location --request GET ''https://api.arkestro.com/api/v2/events'' --header ''Accept: application/json'' --header ''X-Token: <YOUR API TOKEN>'''
  in: header
  name: ApiKeyAuth
  parameter: X-Token
  provisioning: Admin-only, and feature-flagged. Per the OpenAPI description the user must be an admin and must request the API feature be enabled for the tenant; the token is then created at User Settings -> Personal Access Tokens.
  sources:
  - openapi/arkestro-api-v2-openapi.yml
  surface: REST API V2
  type: apiKey
- authorization_response_iss_parameter_supported: true
  flows:
  - authorizationUrl: https://api.arkestro.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.arkestro.com/oauth/token
    scopes:
      mcp:read: null
      mcp:write: null
      offline_access: null
    tokenUrl: https://api.arkestro.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  introspection_endpoint: https://api.arkestro.com/oauth/introspect
  issuer: https://api.arkestro.com
  name: OAuth2
  openid_connect: false
  pkce:
    code_challenge_methods_supported:
    - S256
    evidence: 'An unparameterized GET to /oauth/authorize returns HTTP 400 "invalid_request: code_challenge with code_challenge_method=S256 is required", so PKCE S256 is enforced, not merely advertised.'
    required: true
  response_types_supported:
  - code
  revocation_endpoint: https://api.arkestro.com/oauth/revoke
  sources:
  - well-known/arkestro-oauth-authorization-server.json
  surface: Remote MCP server (https://api.arkestro.com/api/v2/mcp)
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfo_endpoint: null
slug: arkestro-authentication
source_filename: arkestro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/arkestro-api-v2-openapi.yml\ndocs: https://api.arkestro.com/api-docs\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Arkestro runs two distinct auth surfaces that do not overlap. The REST API V2 is\n    API-key only (an admin-issued Personal Access Token in an X-Token header, declared as\n    the sole securityScheme in the published OpenAPI). The remote MCP server at\n    /api/v2/mcp is OAuth 2.1 only, advertised through RFC 8414 authorization-server\n    metadata with PKCE S256 required. Neither surface accepts the other's credential.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Token\n  surface: REST API V2\n  sources:\n  - openapi/arkestro-api-v2-openapi.yml\n  provisioning: >-\n    Admin-only, and feature-flagged. Per the OpenAPI description the user must be an admin\n    and must request the API feature\
  \ be enabled for the tenant; the token is then created at\n    User Settings -> Personal Access Tokens.\n  example_usage: >-\n    curl --location --request GET 'https://api.arkestro.com/api/v2/events'\n    --header 'Accept: application/json' --header 'X-Token: <YOUR API TOKEN>'\n- name: OAuth2\n  type: oauth2\n  surface: Remote MCP server (https://api.arkestro.com/api/v2/mcp)\n  sources:\n  - well-known/arkestro-oauth-authorization-server.json\n  issuer: https://api.arkestro.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.arkestro.com/oauth/authorize\n    tokenUrl: https://api.arkestro.com/oauth/token\n    refreshUrl: https://api.arkestro.com/oauth/token\n    scopes:\n      mcp:read: null\n      mcp:write: null\n      offline_access: null\n  revocation_endpoint: https://api.arkestro.com/oauth/revoke\n  introspection_endpoint: https://api.arkestro.com/oauth/introspect\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n\
  \  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  pkce:\n    required: true\n    code_challenge_methods_supported:\n    - S256\n    evidence: >-\n      An unparameterized GET to /oauth/authorize returns HTTP 400\n      \"invalid_request: code_challenge with code_challenge_method=S256 is required\",\n      so PKCE S256 is enforced, not merely advertised.\n  authorization_response_iss_parameter_supported: true\n  userinfo_endpoint: null\n  openid_connect: false\ngaps:\n- The published OpenAPI declares only ApiKeyAuth; the oauth2 surface is not represented in\n  any spec, so a generated client cannot discover it from the contract alone.\n- No /.well-known/oauth-protected-resource (RFC 9728) document, so an MCP client cannot\n  discover the authorization server from the protected resource in the standard way.\n- No documented token rotation, expiry, or scope model for the X-Token personal access token.\nx-evidence:\n- url: https://api.arkestro.com/api-docs/v2/openapi.yaml\n\
  \  http_status: 200\n  fetched: '2026-08-06'\n- url: https://api.arkestro.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-06'\n- url: https://api.arkestro.com/oauth/authorize\n  http_status: 400\n  fetched: '2026-08-06'\n  note: PKCE enforcement check\n"
source_yaml_url: https://artifacts.apis.io/arkestro/authentication/arkestro-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Procurement
- Sourcing
- Supply Chain
- Spend Management
- eSourcing
- Supplier Management
- Purchase Orders
- procurement-analytics
- Enterprise Software
- predictive-procurement
- MCP
- Webhook
---
