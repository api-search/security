---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hockeystack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HockeyStack secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HockeyStack
provider_slug: hockeystack
scheme_count: 2
schemes:
- base_url: https://app.hockeystack.com/api/revenue-agents/v1
  description: 'Long-lived workspace API token presented as an Authorization: Bearer header. Tokens are formatted hsr_live_<hex> and are issued from HockeyStack workspace settings. GET /health accepts unauthenticated requests; every other operation requires the token. GET /me introspects the token and returns its workspace.'
  env_var: HOCKEYSTACK_API_TOKEN
  expiry: not published
  introspection_endpoint: GET /me
  name: RevenueAgentsBearerToken
  rotation_policy: not published
  scheme: bearer
  scoping: No scope or permission model is published for these tokens — a token appears to carry full workspace access across agents, conversations, tasks and credits.
  sources:
  - https://www.npmjs.com/package/hockeystack-revenue-agents-mcp
  status: current
  surface: HockeyStack Revenue Agents API v1
  token_format: hsr_live_<hex>
  type: http
  unauthenticated_operations:
  - GET /health
- description: OAuth 2.0 authorization-code flow (PKCE / S256) protecting the hosted Omni MCP server. Supports refresh tokens and RFC 7591 dynamic client registration. Access tokens are presented as Bearer tokens against the protected resource https://hockeystack.com/api/mcp/omni.
  flows:
  - authorizationUrl: https://hockeystack.com/api/mcp/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://hockeystack.com/api/mcp/oauth/token
    scopes:
      omni:tools: Access to HockeyStack Omni agent tools
    tokenUrl: https://hockeystack.com/api/mcp/oauth/token
  name: OmniOAuth2
  rechecked: '2026-08-13'
  registration_endpoint: https://hockeystack.com/api/mcp/oauth/register
  revocation_endpoint: https://hockeystack.com/api/mcp/oauth/revoke
  sources:
  - well-known/hockeystack-oauth-authorization-server.json
  status: discovery-withdrawn
  status_detail: The endpoints above were read from RFC 8414 metadata served at app.hockeystack.com on 2026-07-19. On 2026-08-13 that metadata document, and every other /.well-known/ path, returns 404 on every HockeyStack host. The /api/mcp/oauth/* endpoints themselves still answer (302 to login), so the server appears to still exist — but an MCP client can no longer DISCOVER it, and an unauthenticated POST to the MCP endpoint returns a session-login redirect rather than the spec-required 401 + WWW-Authenticate challenge. Re-probe before relying on this scheme.
  surface: HockeyStack Omni MCP server
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: hockeystack-authentication
source_filename: hockeystack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  hockeystack-revenue-agents-mcp@1.1.0 README + build/index.js (first-party) and\n  well-known/hockeystack-oauth-authorization-server.json (captured 2026-07-19)\ndocs: https://agents-docs.hockeystack.com/\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  dynamic_client_registration: true\n  bearer_methods:\n  - header\n  surfaces: 2\n  note: >-\n    Two independent auth systems for two independent surfaces. The REST API uses a\n    long-lived workspace API token; the hosted MCP server uses OAuth. They do not\n    interoperate — an OAuth token will not call the REST API and an hsr_live_ token\n    will not call the Omni MCP server.\nschemes:\n- name: RevenueAgentsBearerToken\n  type: http\n  scheme: bearer\n  surface: HockeyStack Revenue Agents API v1\n  base_url: https://app.hockeystack.com/api/revenue-agents/v1\n  description: >-\n    Long-lived workspace API token presented\
  \ as an Authorization: Bearer header.\n    Tokens are formatted hsr_live_<hex> and are issued from HockeyStack workspace\n    settings. GET /health accepts unauthenticated requests; every other operation\n    requires the token. GET /me introspects the token and returns its workspace.\n  token_format: hsr_live_<hex>\n  env_var: HOCKEYSTACK_API_TOKEN\n  introspection_endpoint: GET /me\n  unauthenticated_operations:\n  - GET /health\n  rotation_policy: not published\n  expiry: not published\n  scoping: >-\n    No scope or permission model is published for these tokens — a token appears to\n    carry full workspace access across agents, conversations, tasks and credits.\n  sources:\n  - https://www.npmjs.com/package/hockeystack-revenue-agents-mcp\n  status: current\n- name: OmniOAuth2\n  type: oauth2\n  surface: HockeyStack Omni MCP server\n  description: >-\n    OAuth 2.0 authorization-code flow (PKCE / S256) protecting the hosted Omni MCP\n    server. Supports refresh tokens and RFC 7591\
  \ dynamic client registration.\n    Access tokens are presented as Bearer tokens against the protected resource\n    https://hockeystack.com/api/mcp/omni.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hockeystack.com/api/mcp/oauth/authorize\n    tokenUrl: https://hockeystack.com/api/mcp/oauth/token\n    refreshUrl: https://hockeystack.com/api/mcp/oauth/token\n    scopes:\n      omni:tools: Access to HockeyStack Omni agent tools\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  registration_endpoint: https://hockeystack.com/api/mcp/oauth/register\n  revocation_endpoint: https://hockeystack.com/api/mcp/oauth/revoke\n  sources:\n  - well-known/hockeystack-oauth-authorization-server.json\n  status: discovery-withdrawn\n  status_detail: >-\n    The endpoints above were read from RFC 8414 metadata served at\n    app.hockeystack.com on 2026-07-19. On 2026-08-13 that metadata document, and\n    every other /.well-known/ path, returns 404 on every HockeyStack\
  \ host. The\n    /api/mcp/oauth/* endpoints themselves still answer (302 to login), so the\n    server appears to still exist — but an MCP client can no longer DISCOVER it,\n    and an unauthenticated POST to the MCP endpoint returns a session-login\n    redirect rather than the spec-required 401 + WWW-Authenticate challenge.\n    Re-probe before relying on this scheme.\n  rechecked: '2026-08-13'\nnotes: >-\n  Corrects the prior round, which recorded HockeyStack as having no REST API. It has\n  one — the Revenue Agents API v1 — with its own bearer-token scheme. What it does\n  not have is a published OpenAPI describing it; the API is documented only in the\n  README of the first-party npm MCP package. Product data integrations remain\n  configured through prebuilt in-app connectors (Salesforce, HubSpot, ad platforms,\n  Snowflake, BigQuery, Segment) rather than through this API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hockeystack/refs/heads/main/authentication/hockeystack-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Data
- Marketing Analytics
- Attribution
- Revenue Intelligence
- B2B
- Account Intelligence
- MCP
- AI Agents
---
