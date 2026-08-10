---
api_key_in: []
auth_types:
- oauth2
description: Acrisure publishes no OpenAPI, so this profile is not derived from securitySchemes. It is read directly from the RFC 8414 authorization-server metadata that api.acrisure.com serves anonymously, plus the observed 302 from /oauth/authorize. The single protected resource this covers is the hosted MCP server at https://api.acrisure.com/v1/mcp.
kind: authentication
layout: security
method: probed
name: Acrisure Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Acrisure secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Acrisure
provider_slug: acrisure
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://api.acrisure.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.acrisure.com/oauth/token
    scopes:
      api://bc250bc0-7689-4f21-b164-72a6b57c273b/mcp_user: Application scope for the Acrisure MCP server. Description not published by Acrisure — the scope name is verbatim from scopes_supported.
      offline_access: Standard OIDC scope permitting refresh-token issuance.
    tokenUrl: https://api.acrisure.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.acrisure.com
  jwks_uri: https://login.microsoftonline.com/c2ec94c0-ebd0-4630-aef2-2dcf0eb68ebd/discovery/v2.0/keys
  name: AcrisureOAuth2
  response_modes:
  - query
  response_types:
  - code
  source: https://api.acrisure.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: acrisure-authentication
source_filename: acrisure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://api.acrisure.com/.well-known/oauth-authorization-server\ndescription: >-\n  Acrisure publishes no OpenAPI, so this profile is not derived from securitySchemes. It is\n  read directly from the RFC 8414 authorization-server metadata that api.acrisure.com\n  serves anonymously, plus the observed 302 from /oauth/authorize. The single protected\n  resource this covers is the hosted MCP server at https://api.acrisure.com/v1/mcp.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  identity_provider: Microsoft Entra ID\n  pkce_required_methods:\n  - S256\nschemes:\n- name: AcrisureOAuth2\n  type: oauth2\n  source: https://api.acrisure.com/.well-known/oauth-authorization-server\n  issuer: https://api.acrisure.com\n  jwks_uri: https://login.microsoftonline.com/c2ec94c0-ebd0-4630-aef2-2dcf0eb68ebd/discovery/v2.0/keys\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.acrisure.com/oauth/authorize\n\
  \    tokenUrl: https://api.acrisure.com/oauth/token\n    refreshUrl: https://api.acrisure.com/oauth/token\n    scopes:\n      api://bc250bc0-7689-4f21-b164-72a6b57c273b/mcp_user: >-\n        Application scope for the Acrisure MCP server. Description not published by\n        Acrisure — the scope name is verbatim from scopes_supported.\n      offline_access: Standard OIDC scope permitting refresh-token issuance.\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  response_modes:\n  - query\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  code_challenge_methods:\n  - S256\nprotected_resources:\n- url: https://api.acrisure.com/v1/mcp\n  kind: MCPServer\n  artifact: mcp/acrisure-mcp.yml\n  observed_status: 403\nnotes:\n- >-\n  The authorization and token endpoints are Acrisure-branded proxies on api.acrisure.com;\n  /oauth/authorize 302s to\n  login.microsoftonline.com/c2ec94c0-ebd0-4630-aef2-2dcf0eb68ebd, so the actual\n\
  \  authorization server is Microsoft Entra ID and the tenant is Acrisure's own.\n- >-\n  Client registration is not self-serve. There is no dynamic client registration endpoint\n  in the metadata and no public sign-up for API credentials, so a client_id must be issued\n  out of band by Acrisure.\n- >-\n  No OpenID Connect discovery document is served\n  (/.well-known/openid-configuration returns 404 on api.acrisure.com), so this is OAuth 2.0\n  authorization-server metadata only, not OIDC.\n- >-\n  No documentation page for authentication exists on any Acrisure host — this profile is\n  built entirely from machine-readable discovery metadata, not from prose docs.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://api.acrisure.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n    file: well-known/acrisure-oauth-authorization-server.json\n  - url: https://api.acrisure.com/oauth/authorize\n    http_status: 302\n    location:\
  \ https://login.microsoftonline.com/c2ec94c0-ebd0-4630-aef2-2dcf0eb68ebd/oauth2/v2.0/authorize\n  - url: https://api.acrisure.com/oauth/token\n    http_status: 405\n    note: Method Not Allowed on GET — the endpoint exists and accepts POST only.\n  - url: https://api.acrisure.com/.well-known/openid-configuration\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acrisure/refs/heads/main/authentication/acrisure-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- insurance
- insurance-brokerage
- fintech
- employee-benefits
- payroll-hr
- reinsurance
- risk-management
- cybersecurity
- mortgage
- surety-bonds
- mcp
- oauth2
---
