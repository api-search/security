---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Winnai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Winn.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Winn.ai
provider_slug: winnai
scheme_count: 2
schemes:
- applies_to: https://app.winn.ai/mcp
  authorization_response_iss_parameter_supported: true
  bearer_methods_supported:
  - header
  dynamic_client_registration:
    endpoint: https://app.winn.ai/api/auth/oauth/register
    spec: RFC 7591
    supported: true
  flows:
    authorization_code:
      authorization_url: https://app.winn.ai/api/auth/oauth/authorize
      pkce_required_methods:
      - S256
      refresh_supported: true
      scopes:
        sessions:read: Read access to recorded call sessions. Scope name taken verbatim from scopes_supported in the authorization server metadata; WINN.AI publishes no description for it.
      token_url: https://app.winn.ai/api/auth/oauth/token
  id: winnai-app-oauth2
  protected_resource_metadata: https://app.winn.ai/.well-known/oauth-protected-resource
  public_client: true
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  x-evidence:
    fetched: '2026-08-13'
    http_status: 200
    url: https://app.winn.ai/.well-known/oauth-authorization-server
- applies_to: https://winn.ai/wp-json/mcp/mcp-oauth-server
  bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  first_party: true
  flows:
    authorization_code:
      authorization_url: https://winn.ai/oauth/authorize
      pkce_required_methods:
      - S256
      refresh_supported: true
      revocation_url: https://winn.ai/oauth/revoke
      scopes:
        mcp: Single coarse scope covering the WordPress MCP surface. No description published.
      token_url: https://winn.ai/oauth/token
  id: winnai-wordpress-oauth2
  note: Belongs to the WordPress CMS behind the marketing site, not to the WINN.AI sales product. Kept separate so the product auth model is not overstated.
  product_surface: false
  public_client: true
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  x-evidence:
    fetched: '2026-08-13'
    http_status: 200
    url: https://winn.ai/.well-known/oauth-authorization-server
slug: winnai-authentication
source_filename: winnai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://app.winn.ai/.well-known/oauth-authorization-server and\n  https://winn.ai/.well-known/oauth-authorization-server (RFC 8414), plus live\n  401 responses from https://app.winn.ai/mcp and https://app.winn.ai/api/*\ndocs: null\ndocs_note: >-\n  WINN.AI publishes no developer authentication page. The entire auth model below\n  was read from machine-readable OAuth metadata the company serves, not from\n  human documentation.\n\nsummary: >-\n  WINN.AI runs two independent OAuth 2.0 authorization servers, one per host. The\n  product application (app.winn.ai) protects its MCP endpoint with authorization\n  code + PKCE and supports dynamic client registration; the marketing site\n  (winn.ai) runs the WordPress MCP plugin's own authorization server. Everything\n  under app.winn.ai/api is bearer-gated with no anonymous surface at all.\n\nschemes:\n- id: winnai-app-oauth2\n  type: oauth2\n  applies_to: https://app.winn.ai/mcp\n\
  \  flows:\n    authorization_code:\n      authorization_url: https://app.winn.ai/api/auth/oauth/authorize\n      token_url: https://app.winn.ai/api/auth/oauth/token\n      refresh_supported: true\n      pkce_required_methods:\n      - S256\n      scopes:\n        sessions:read: >-\n          Read access to recorded call sessions. Scope name taken verbatim from\n          scopes_supported in the authorization server metadata; WINN.AI publishes\n          no description for it.\n  token_endpoint_auth_methods_supported:\n  - none\n  public_client: true\n  dynamic_client_registration:\n    supported: true\n    endpoint: https://app.winn.ai/api/auth/oauth/register\n    spec: RFC 7591\n  authorization_response_iss_parameter_supported: true\n  bearer_methods_supported:\n  - header\n  protected_resource_metadata: https://app.winn.ai/.well-known/oauth-protected-resource\n  x-evidence:\n    url: https://app.winn.ai/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-13'\n\
  \n- id: winnai-wordpress-oauth2\n  type: oauth2\n  applies_to: https://winn.ai/wp-json/mcp/mcp-oauth-server\n  first_party: true\n  product_surface: false\n  flows:\n    authorization_code:\n      authorization_url: https://winn.ai/oauth/authorize\n      token_url: https://winn.ai/oauth/token\n      revocation_url: https://winn.ai/oauth/revoke\n      refresh_supported: true\n      pkce_required_methods:\n      - S256\n      scopes:\n        mcp: >-\n          Single coarse scope covering the WordPress MCP surface. No description\n          published.\n  token_endpoint_auth_methods_supported:\n  - none\n  public_client: true\n  client_id_metadata_document_supported: true\n  bearer_methods_supported:\n  - header\n  x-evidence:\n    url: https://winn.ai/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-13'\n  note: >-\n    Belongs to the WordPress CMS behind the marketing site, not to the WINN.AI\n    sales product. Kept separate so the product auth model\
  \ is not overstated.\n\nobserved_challenges:\n- url: https://app.winn.ai/mcp\n  method: POST\n  http_status: 401\n  body: '{\"error\":\"Missing credential\"}'\n  www_authenticate: null\n  deviation: >-\n    No WWW-Authenticate header is returned, so an MCP client cannot discover the\n    authorization server from the challenge as RFC 9728 and the MCP authorization\n    specification intend. Discovery only works if the client already knows to\n    fetch /.well-known/oauth-protected-resource.\n- url: https://app.winn.ai/api/v1/sessions\n  method: GET\n  http_status: 401\n  body: '{\"statusCode\":401,\"timestamp\":\"2026-08-14T02:24:23Z\",\"path\":\"/api/v1/sessions\",\"message\":\"Unauthorized\"}'\n  www_authenticate: null\n  note: >-\n    Every probed path under https://app.winn.ai/api returns this same envelope,\n    including /api, /api/docs, /api/openapi, /api/swagger.json and\n    /api/v1/openapi.json. There is no anonymous endpoint and no unauthenticated\n    spec route.\n\napi_keys:\
  \ false\napi_keys_note: >-\n  No API key scheme is documented or observed. WINN.AI's pricing page lists \"API\n  access\" as an Enterprise-tier feature reached through sales, and every observed\n  credential is an OAuth bearer token.\n\nmtls: false\nopenid_connect: false\nopenid_connect_note: >-\n  /.well-known/openid-configuration returns 404 on www.winn.ai and the SPA shell\n  on app.winn.ai. Neither authorization server advertises OIDC. Note that the\n  pricing page separately advertises SAML SSO with Okta for end-user login on the\n  Enterprise plan — that is workforce SSO into the product, not an API auth\n  scheme, and no SAML metadata is published.\n\nrelated:\n- scopes/winnai-scopes.yml\n- mcp/winnai-mcp.yml\n- well-known/winnai-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/winnai/refs/heads/main/authentication/winnai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Sales
- Artificial Intelligence
- Revenue
- CRM
- Sales Enablement
- Conversation Intelligence
- Productivity
---
