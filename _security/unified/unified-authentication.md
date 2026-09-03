---
api_key_in: []
api_specs:
- filename: unified-mcp-service-openapi.json
  format: json
  label: Unified MCP Service
  slug: unified-mcp-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified/refs/heads/main/openapi/unified-mcp-service-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Unified Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unified declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Unified
provider_slug: unified
scheme_count: 2
schemes:
- applies_to:
  - https://mcp.unified.com/mcp
  code_challenge_methods:
  - S256
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.unified.com/authorize
      refreshUrl: https://mcp.unified.com/token
      scopes:
        openid: The only scope advertised by the authorization server metadata.
      tokenUrl: https://mcp.unified.com/token
  format: Bearer <token>
  grant_types:
  - authorization_code
  - refresh_token
  in: header
  issuer: https://mcp.unified.com/
  name: mcp_oauth_bearer
  parameter: Authorization
  registration_endpoint: https://mcp.unified.com/register
  revocation_endpoint: https://mcp.unified.com/revoke
  standard: OAuth 2.0 with PKCE; discovery per RFC 8414, protected resource per RFC 9728, bearer usage and challenge per RFC 6750, dynamic registration per RFC 7591
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- applies_to:
  - https://api.unified.com/
  - https://api.unified.com/health
  - https://api.unified.com/health/ready
  - https://api.unified.com/health/live
  - https://api.unified.com/openapi.json
  name: none
  note: The root, health and description endpoints answer 200 anonymously; they carry no security requirement in the spec and none was observed.
  type: none
slug: unified-authentication
source_filename: unified-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://mcp.unified.com/.well-known/oauth-authorization-server,\n  https://mcp.unified.com/.well-known/oauth-protected-resource/mcp, and the RFC 6750 challenge\n  returned by an anonymous POST to https://mcp.unified.com/mcp. Probed 2026-09-02.\nnote: >-\n  Derived from live discovery documents rather than from the OpenAPI, because the published\n  OpenAPI (openapi/unified-mcp-service-openapi.json) declares NO securitySchemes at all — it\n  describes only unauthenticated root and health probes. Unified's real authentication surface is\n  the OAuth authorization server fronting the MCP endpoint. Unified publishes no anonymous\n  developer authentication page; docs.unified.com is behind SSO.\nschemes:\n- name: mcp_oauth_bearer\n  type: oauth2\n  standard: OAuth 2.0 with PKCE; discovery per RFC 8414, protected resource per RFC 9728,\n    bearer usage and challenge per RFC 6750, dynamic registration per RFC 7591\n  in: header\n\
  \  parameter: Authorization\n  format: Bearer <token>\n  issuer: https://mcp.unified.com/\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.unified.com/authorize\n      tokenUrl: https://mcp.unified.com/token\n      refreshUrl: https://mcp.unified.com/token\n      scopes:\n        openid: The only scope advertised by the authorization server metadata.\n  code_challenge_methods:\n  - S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  revocation_endpoint: https://mcp.unified.com/revoke\n  registration_endpoint: https://mcp.unified.com/register\n  dynamic_client_registration: true\n  applies_to:\n  - https://mcp.unified.com/mcp\n- name: none\n  type: none\n  applies_to:\n  - https://api.unified.com/\n  - https://api.unified.com/health\n  - https://api.unified.com/health/ready\n  - https://api.unified.com/health/live\n  - https://api.unified.com/openapi.json\n  note: >-\n \
  \   The root, health and description endpoints answer 200 anonymously; they carry no security\n    requirement in the spec and none was observed.\ncustomer_application:\n  url: https://get.unified.com/login\n  model: session sign-in to the Unified web application; every /.well-known/ path on that host\n    302s into the login flow.\n  observed_status: 200\ndocumentation:\n  url: https://docs.unified.com/\n  observed_status: 200\n  effective: >-\n    307/redirect chain into https://iheartmedia.unified.com/login — a GitBook space behind single\n    sign-on. No anonymous authentication reference could be read.\nx-evidence:\n- fetched: '2026-09-02'\n  url: https://mcp.unified.com/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-09-02'\n  url: https://mcp.unified.com/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n- fetched: '2026-09-02'\n  url: https://mcp.unified.com/mcp\n  http_status: 401\n- fetched: '2026-09-02'\n  url: https://docs.unified.com/\n\
  \  http_status: 200\n  effective_url: https://iheartmedia.unified.com/login?next=%2Fiheartmedia%2Fidentity%2Fauth%2Fgitbook%2Fsso\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unified/refs/heads/main/authentication/unified-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- Social Media
- Digital Advertising
- Marketing
- Analytics
- Media
- Agents
- MCP
---
