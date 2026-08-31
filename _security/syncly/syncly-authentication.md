---
api_key_in: []
api_specs:
- filename: syncly-health-api-openapi.yml
  format: yaml
  label: Syncly Health API
  slug: syncly-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/openapi/syncly-health-api-openapi.yml
- filename: syncly-well-known-api-openapi.yml
  format: yaml
  label: Syncly .well Known API
  slug: syncly-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/openapi/syncly-well-known-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Syncly Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Syncly secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Syncly
provider_slug: syncly
scheme_count: 1
schemes:
- description: Programmatic access to a Syncly workspace goes through the Syncly Social MCP server at https://mcp.syncly.app/mcp, which is an OAuth 2.1 protected resource. Clients discover the authorization server from the resource metadata document, register dynamically, run an authorization-code flow with PKCE (S256), and present the resulting access token as an HTTP Authorization Bearer header. Token endpoint auth method is "none", which is the public client profile expected of MCP clients. In practice end users trigger this flow from Settings > My Account > Connected Apps inside the Syncly app rather than pasting a URL.
  flows:
  - authorizationUrl: https://social-server.syncly.app/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://social-server.syncly.app/oauth/register
    revocationUrl: https://social-server.syncly.app/oauth/revoke
    scopes:
      offline_access: Issue a refresh token so the client can renew access without re-consent
      syncly:read: Read access to the connected Syncly workspace
    tokenUrl: https://social-server.syncly.app/oauth/token
  name: SynclySocialOAuth
  sources:
  - https://mcp.syncly.app/.well-known/oauth-protected-resource
  - https://social-server.syncly.app/.well-known/oauth-authorization-server
  type: oauth2
slug: syncly-authentication
source_filename: syncly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://social-server.syncly.app/.well-known/oauth-authorization-server\ndocs: https://syncly-a76215af.mintlify.app/en/start/connect-mcp-clients\nsupersedes: >-\n  The 2026-07-21 round recorded a \"workspace MCP connection URL\" scheme and stated that no\n  OAuth surface was documented. That was wrong. Syncly runs a full OAuth 2.1 authorization\n  server at https://social-server.syncly.app, discoverable per RFC 8414, and the MCP resource\n  server advertises it per RFC 9728. Corrected here from live probes.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_methods_supported: [header]\n  dynamic_client_registration: true\n  pkce_required_methods: [S256]\nschemes:\n- name: SynclySocialOAuth\n  type: oauth2\n  description: >-\n    Programmatic access to a Syncly workspace goes through the Syncly Social MCP server at\n    https://mcp.syncly.app/mcp, which is an OAuth 2.1 protected resource.\
  \ Clients discover the\n    authorization server from the resource metadata document, register dynamically, run an\n    authorization-code flow with PKCE (S256), and present the resulting access token as an\n    HTTP Authorization Bearer header. Token endpoint auth method is \"none\", which is the public\n    client profile expected of MCP clients. In practice end users trigger this flow from\n    Settings > My Account > Connected Apps inside the Syncly app rather than pasting a URL.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://social-server.syncly.app/oauth/authorize\n    tokenUrl: https://social-server.syncly.app/oauth/token\n    revocationUrl: https://social-server.syncly.app/oauth/revoke\n    registrationUrl: https://social-server.syncly.app/oauth/register\n    scopes:\n      syncly:read: Read access to the connected Syncly workspace\n      offline_access: Issue a refresh token so the client can renew access without re-consent\n  sources:\n  - https://mcp.syncly.app/.well-known/oauth-protected-resource\n\
  \  - https://social-server.syncly.app/.well-known/oauth-authorization-server\nauthorization_server:\n  issuer: https://social-server.syncly.app\n  metadata: well-known/syncly-oauth-authorization-server.json\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\nprotected_resource:\n  resource: https://mcp.syncly.app/mcp\n  metadata: well-known/syncly-oauth-protected-resource.json\n  authorization_servers: [https://social-server.syncly.app]\n  scopes_supported: [syncly:read]\nunauthenticated_behavior:\n  http_status: 401\n  body: JSON-RPC 2.0 error object, code -32001, message \"Unauthorized\"\n  challenge_header: mcp/www_authenticate carried inside the JSON-RPC error _meta block\n  note: >-\n    The Bearer challenge is delivered in the JSON-RPC error payload rather than a plain\n    WWW-Authenticate response\
  \ header, which is the MCP-specific shape of the RFC 9728 challenge.\nno_rest_api: >-\n  Syncly publishes no general-purpose REST API and no API-key issuance flow. The only\n  machine-readable contract on its own hosts is openapi/syncly-social-mcp-openapi.json, which\n  documents the MCP server's discovery and health endpoints, not the product data surface.\nx-evidence:\n- url: https://social-server.syncly.app/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://mcp.syncly.app/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://mcp.syncly.app/mcp\n  http_status: 401\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/authentication/syncly-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Social Intelligence
- Social Listening
- Customer Feedback
- Voice of Customer
- Creator Marketing
- Analytics
- Artificial Intelligence
- MCP
---
