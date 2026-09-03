---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Vanderhall Motor Works Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vanderhall Motor Works declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vanderhall Motor Works
provider_slug: vanderhall-motor-works
scheme_count: 1
schemes:
- applies_to: https://portal.vanderhallusa.com/mcp
  bearer_token:
    observed_failure: 'Requests without a token return HTTP 200 carrying JSON-RPC error -32001 "Unauthorized: missing bearer token". Note that the transport status is 200, not 401 — a client must read the JSON-RPC error envelope, not the HTTP status, to detect an auth failure.'
    transport: Authorization header
  client_authentication:
    note: Public clients only — the authorization server advertises `none` as its sole token-endpoint auth method, which is the expected posture for MCP clients paired with PKCE and dynamic registration.
    token_endpoint_auth_methods:
    - none
  dynamic_client_registration:
    endpoint: https://portal.vanderhallusa.com/oauth/register
    observed: A GET returns HTTP 400 {"error":"invalid_client_metadata","error_description":"redirect_uris is required and must be a non-empty array"} — the endpoint is live and validating.
    spec: RFC 7591
    supported: true
  flows:
    authorizationCode:
      authorizationUrl: https://portal.vanderhallusa.com/shared/oauth_authorize
      refreshUrl: https://portal.vanderhallusa.com/oauth/token
      scopes:
        mcp: Access the Vanderhall Admin Portal MCP endpoint.
      tokenUrl: https://portal.vanderhallusa.com/oauth/token
  name: mcp_oauth2
  pkce:
    required_methods:
    - S256
  type: oauth2
slug: vanderhall-motor-works-authentication
source_filename: vanderhall-motor-works-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://portal.vanderhallusa.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived entirely from the two live OAuth discovery documents Vanderhall serves at\n  portal.vanderhallusa.com — there is no OpenAPI to read securitySchemes from and no public\n  authentication documentation page anywhere on the Vanderhall estate.\nschemes:\n- name: mcp_oauth2\n  type: oauth2\n  applies_to: https://portal.vanderhallusa.com/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://portal.vanderhallusa.com/shared/oauth_authorize\n      tokenUrl: https://portal.vanderhallusa.com/oauth/token\n      refreshUrl: https://portal.vanderhallusa.com/oauth/token\n      scopes:\n        mcp: Access the Vanderhall Admin Portal MCP endpoint.\n  pkce:\n    required_methods: [S256]\n  client_authentication:\n    token_endpoint_auth_methods: [none]\n    note: >-\n      Public clients only — the authorization server advertises `none`\
  \ as its sole token-endpoint auth\n      method, which is the expected posture for MCP clients paired with PKCE and dynamic registration.\n  dynamic_client_registration:\n    supported: true\n    spec: RFC 7591\n    endpoint: https://portal.vanderhallusa.com/oauth/register\n    observed: >-\n      A GET returns HTTP 400 {\"error\":\"invalid_client_metadata\",\"error_description\":\"redirect_uris is\n      required and must be a non-empty array\"} — the endpoint is live and validating.\n  bearer_token:\n    transport: Authorization header\n    observed_failure: >-\n      Requests without a token return HTTP 200 carrying JSON-RPC error -32001 \"Unauthorized: missing\n      bearer token\". Note that the transport status is 200, not 401 — a client must read the JSON-RPC\n      error envelope, not the HTTP status, to detect an auth failure.\ndiscovery:\n- spec: RFC 8414 OAuth 2.0 Authorization Server Metadata\n  url: https://portal.vanderhallusa.com/.well-known/oauth-authorization-server\n\
  \  status: 200\n- spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  url: https://portal.vanderhallusa.com/.well-known/oauth-protected-resource\n  status: 200\n- spec: OpenID Connect Discovery\n  url: https://portal.vanderhallusa.com/.well-known/openid-configuration\n  status: 404\n  note: Plain OAuth 2.1-style authorization only; no OIDC layer is advertised.\nother_surfaces:\n- surface: https://dealer.vanderhallusa.com/\n  auth: HTML form login (username + password), no public API auth documented\n  status: 200\n- surface: https://portal.vanderhallusa.com/\n  auth: HTML form login (username + password)\n  status: 200\n- surface: https://dealer.vanderhallusa.com/api\n  auth: unknown\n  status: 200\n  note: >-\n    An undocumented internal router that answers \"INVALID API CALL. api\" (21 bytes) at /api and /api/\n    and 404s on every child path probed (/api/v1, /api/dealers, /api/inventory, /api/help, /api/docs).\n    No contract, no reference, no auth scheme is published for it;\
  \ recorded as observed, not derived.\ndocs: null\ndocs_note: Vanderhall publishes no authentication documentation page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanderhall-motor-works/refs/heads/main/authentication/vanderhall-motor-works-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Automotive
- Manufacturing
- Electric Vehicles
- Powersports
- Autocycles
- Dealer Network
- Model Context Protocol
- Utah
---
