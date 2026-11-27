---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloche Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloche declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloche
provider_slug: cloche-dev
scheme_count: 1
schemes:
- authorization_server: https://sleek-marigold-65.authkit.app
  authorization_server_metadata: https://sleek-marigold-65.authkit.app/.well-known/oauth-authorization-server
  bearer_methods:
  - header
  description: 'Docs: "Let your client run the authorization-code flow with PKCE that the metadata advertises." Unauthenticated calls to /mcp (initialize included) answer 401 with WWW-Authenticate: Bearer resource_metadata="https://mcp.cloche.dev/.well-known/oauth-protected-resource". Verification is a successful list_apps call.'
  dynamic_client_registration: true
  flows:
  - authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  name: Cloche MCP OAuth (WorkOS AuthKit)
  pkce: S256
  protected_resource: https://mcp.cloche.dev/mcp
  resource_metadata: https://mcp.cloche.dev/.well-known/oauth-protected-resource
  token_audience: https://mcp.cloche.dev/mcp
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: cloche-dev-authentication
source_filename: cloche-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cloche.dev/auth.md\ndocs: https://cloche.dev/auth.md\nname: Cloche authentication\nschemes:\n- type: oauth2\n  name: Cloche MCP OAuth (WorkOS AuthKit)\n  flows: [authorization_code]\n  pkce: S256\n  bearer_methods: [header]\n  protected_resource: https://mcp.cloche.dev/mcp\n  resource_metadata: https://mcp.cloche.dev/.well-known/oauth-protected-resource\n  authorization_server: https://sleek-marigold-65.authkit.app\n  authorization_server_metadata: https://sleek-marigold-65.authkit.app/.well-known/oauth-authorization-server\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  dynamic_client_registration: true\n  token_audience: https://mcp.cloche.dev/mcp\n  description: 'Docs: \"Let your client run the authorization-code flow with PKCE that the metadata advertises.\" Unauthenticated\
  \ calls to /mcp (initialize included) answer 401 with WWW-Authenticate: Bearer resource_metadata=\"https://mcp.cloche.dev/.well-known/oauth-protected-resource\". Verification is a successful list_apps call.'\ndiscovery:\n- url: https://cloche.dev/.well-known/oauth-protected-resource\n  http_status: 200\n  note: redirects to https://mcp.cloche.dev/.well-known/oauth-protected-resource (RFC 9728)\n- url: https://cloche.dev/.well-known/oauth-authorization-server\n  http_status: 200\n  note: redirects to the AuthKit issuer metadata\nnote: The docs state there is no WorkOS auth.md agent-registration (agent_auth) endpoint. Grant/scope values were read from the advertised metadata documents via GET on 2026-11-04.\n"
source_yaml_url: https://artifacts.apis.io/cloche-dev/authentication/cloche-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- MCP
- Ai Apps
- Governance
- Low-Code
- Internal Tools
- Agents
---
