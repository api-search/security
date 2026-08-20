---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Serviceup Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ServiceUp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ServiceUp
provider_slug: serviceup
scheme_count: 1
schemes:
- description: OAuth 2.1 authorization-code flow with PKCE protecting the ServiceUp MCP server. Access tokens are presented as a Bearer token in the Authorization header.
  flows:
  - authorizationUrl: https://auth.serviceup.com/api/auth/oauth2/authorize
    flow: authorizationCode
    scopes:
    - mcp:read
    - mcp:write
    - offline_access
    tokenUrl: https://auth.serviceup.com/api/auth/oauth2/token
  name: ServiceUpOAuth2
  sources:
  - well-known/serviceup-oauth-authorization-server.json
  - well-known/serviceup-oauth-protected-resource-mcp.json
  type: oauth2
slug: serviceup-authentication
source_filename: serviceup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://auth.serviceup.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  ServiceUp publishes no developer documentation for its API. This profile is built\n  entirely from the machine-readable OAuth metadata the provider serves anonymously\n  (RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata),\n  plus the WWW-Authenticate challenge returned by the MCP endpoint itself. No\n  OpenAPI or securitySchemes were found to derive from.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  bearer_methods:\n  - header\n  pkce: required-by-metadata\nschemes:\n- name: ServiceUpOAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code flow with PKCE protecting the ServiceUp MCP server.\n    Access tokens are presented as a Bearer token in the Authorization header.\n  sources:\n  - well-known/serviceup-oauth-authorization-server.json\n\
  \  - well-known/serviceup-oauth-protected-resource-mcp.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.serviceup.com/api/auth/oauth2/authorize\n    tokenUrl: https://auth.serviceup.com/api/auth/oauth2/token\n    scopes:\n    - mcp:read\n    - mcp:write\n    - offline_access\nauthorization_server:\n  issuer: https://auth.serviceup.com\n  metadata_url: https://auth.serviceup.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://auth.serviceup.com/api/auth/oauth2/authorize\n  token_endpoint: https://auth.serviceup.com/api/auth/oauth2/token\n  jwks_uri: https://auth.serviceup.com/api/auth/jwks\n  registration_endpoint: null\n  dynamic_client_registration: false\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  code_challenge_methods_supported:\n  - S256\n  scopes_supported:\n\
  \  - mcp:read\n  - mcp:write\n  - offline_access\nprotected_resources:\n- resource: https://api.serviceup.com/mcp\n  metadata_url: https://api.serviceup.com/.well-known/oauth-protected-resource/mcp\n  authorization_servers:\n  - https://auth.serviceup.com\n  scopes_supported:\n  - mcp:read\n  - mcp:write\n  bearer_methods_supported:\n  - header\nsigning_keys:\n  jwks_url: https://auth.serviceup.com/api/auth/jwks\n  file: well-known/serviceup-jwks.json\n  algorithms:\n  - EdDSA\n  curves:\n  - Ed25519\n  key_count: 1\nobservations:\n- >-\n  No registration_endpoint is advertised, so RFC 7591 dynamic client registration is\n  not available; MCP clients need a client_id issued out of band by ServiceUp.\n- >-\n  token_endpoint_auth_methods_supported includes \"none\", which permits public clients\n  using PKCE.\n- >-\n  No /.well-known/openid-configuration is served (auth.serviceup.com returns a Next.js\n  HTML 404 page), so this is plain OAuth 2.1, not OpenID Connect.\nx-evidence:\n- url:\
  \ https://auth.serviceup.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-05'\n- url: https://api.serviceup.com/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n  content_type: application/json; charset=utf-8\n  fetched: '2026-08-05'\n- url: https://auth.serviceup.com/api/auth/jwks\n  http_status: 200\n  content_type: application/json\n  fetched: '2026-08-05'\n- url: https://auth.serviceup.com/.well-known/openid-configuration\n  http_status: 404\n  content_type: text/html; charset=utf-8\n  fetched: '2026-08-05'\n- url: https://auth.serviceup.com/api/auth/oauth2/register\n  http_status: 404\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serviceup/refs/heads/main/authentication/serviceup-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fleet Management
- Vehicle Repair
- Automotive
- Insurance
- Maintenance
- Agentic AI
- MCP
- Transportation
---
