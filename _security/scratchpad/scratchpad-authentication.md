---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Scratchpad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Scratchpad secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Scratchpad
provider_slug: scratchpad
scheme_count: 1
schemes:
- applies_to: https://mcp.clearskies.cc/mcp
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://mcp.clearskies.cc/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://mcp.clearskies.cc/oauth/register
    scopes:
      email: Email address claim
      openid: OpenID Connect subject identifier
      profile: Basic profile claims
    tokenUrl: https://mcp.clearskies.cc/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.clearskies.cc
  name: ClearskiesMCPOAuth
  resource_signing_alg_values_supported:
  - RS256
  response_types_supported:
  - code
  sources:
  - well-known/scratchpad-oauth-authorization-server.json
  - well-known/scratchpad-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: scratchpad-authentication
source_filename: scratchpad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.clearskies.cc/.well-known/oauth-authorization-server\ndocs: https://clearskies.cc/docs/building-with-clearskies/mcp-server\nnote: >-\n  Derived from the live RFC 8414 / RFC 9728 discovery documents rather than an OpenAPI, because\n  Scratchpad publishes no OpenAPI. The only authenticated machine surface the company operates is the\n  Clearskies remote MCP server; the Scratchpad workspace itself authenticates to Salesforce as an\n  OAuth client and inherits Salesforce permissions, but exposes no inbound developer credential.\n\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_methods: [header]\n  dynamic_client_registration: true\n  pkce_required_methods: [S256]\n\nschemes:\n- name: ClearskiesMCPOAuth\n  type: oauth2\n  applies_to: https://mcp.clearskies.cc/mcp\n  sources: [well-known/scratchpad-oauth-authorization-server.json, well-known/scratchpad-oauth-protected-resource.json]\n\
  \  issuer: https://mcp.clearskies.cc\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.clearskies.cc/oauth/authorize\n    tokenUrl: https://mcp.clearskies.cc/oauth/token\n    registrationUrl: https://mcp.clearskies.cc/oauth/register\n    scopes:\n      openid: OpenID Connect subject identifier\n      profile: Basic profile claims\n      email: Email address claim\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  resource_signing_alg_values_supported: [RS256]\n\nprotected_resource:\n  resource: https://mcp.clearskies.cc\n  authorization_servers: [https://mcp.clearskies.cc]\n  bearer_methods_supported: [header]\n  challenge_observed: >-\n    WWW-Authenticate: Bearer realm=\"mcp\", error=\"invalid_request\",\n    error_description=\"missing authorization header\",\n    resource_metadata=\"\
  https://mcp.clearskies.cc/.well-known/oauth-protected-resource\"\n\nend_user_flow:\n  description: >-\n    A Claude workspace admin adds Clearskies as a custom connector using the workspace MCP URL from\n    app.clearskies.cc/settings/mcp-server; each team member then clicks Connect and authenticates\n    against their email domain in the Clearskies app, which completes the OAuth authorization code\n    exchange back to the client.\n  source: https://clearskies.cc/docs/building-with-clearskies/mcp-clients/claude.md\n\nbyok:\n  supported: true\n  description: >-\n    Clearskies workspaces can bring their own AI provider API keys (BYOK) and manage model\n    availability. These are outbound model credentials configured in the app, not an inbound\n    Clearskies API credential.\n  source: https://clearskies.cc/docs/building-with-clearskies/ai-providers.md\n\nx-evidence:\n- fetched: '2026-08-13'\n  url: https://mcp.clearskies.cc/.well-known/oauth-authorization-server\n  http_status: 200\n\
  - fetched: '2026-08-13'\n  url: https://mcp.clearskies.cc/.well-known/oauth-protected-resource\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://mcp.clearskies.cc/mcp\n  http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scratchpad/refs/heads/main/authentication/scratchpad-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Productivity
- Sales
- CRM
- Salesforce
- Revenue Operations
- Artificial Intelligence
- Software-as-a-Service
- MCP
- Agents
- Sales Intelligence
---
