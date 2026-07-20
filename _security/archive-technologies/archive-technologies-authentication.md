---
api_key_in:
- header
auth_types:
- http
- oauth2
description: Archive's public GraphQL API authenticates with a workspace-scoped bearer token generated in the Archive app under Settings -> API (compatible plans only). Every request also carries a WORKSPACE-ID header (workspace UUID) to scope the query to a workspace or agency. Separately, Archive's hosted MCP server uses OAuth 2.0 (authorization code + PKCE) with a single "mcp" scope. No scopes are documented for the direct GraphQL bearer token.
kind: authentication
layout: security
method: searched
name: Archive Technologies Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Archive Technologies secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Archive Technologies
provider_slug: archive-technologies
scheme_count: 3
schemes:
- bearerFormat: opaque token, prefix arch_live_
  description: 'Workspace API token. Passed as `Authorization: Bearer [example key]`. Generated in the Archive UI (Settings -> API). Scoped per workspace/agency; must accompany the WORKSPACE-ID header.'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://api-docs.archive.com
  type: http
- description: Workspace UUID identifying which workspace the token operates against. Required for workspace-scoped queries; passed as a header, never in the request body.
  in: header
  name: workspaceId
  parameterName: WORKSPACE-ID
  sources:
  - https://api-docs.archive.com
  type: apiKey
- description: OAuth 2.0 authorization used by the hosted MCP server (app.archive.com/api/v2/mcp).
  flows:
  - authorizationUrl: https://app.archive.com/oauth/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    registrationUrl: https://app.archive.com/oauth/register
    scopes:
    - mcp
    tokenUrl: https://app.archive.com/oauth/token
  name: mcpOAuth
  sources:
  - https://app.archive.com/.well-known/oauth-authorization-server
  type: oauth2
slug: archive-technologies-authentication
source_filename: archive-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api-docs.archive.com\ndescription: >-\n  Archive's public GraphQL API authenticates with a workspace-scoped bearer token generated\n  in the Archive app under Settings -> API (compatible plans only). Every request also\n  carries a WORKSPACE-ID header (workspace UUID) to scope the query to a workspace or agency.\n  Separately, Archive's hosted MCP server uses OAuth 2.0 (authorization code + PKCE) with a\n  single \"mcp\" scope. No scopes are documented for the direct GraphQL bearer token.\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque token, prefix arch_live_\n  in: header\n  header: Authorization\n  description: >-\n    Workspace API token. Passed as `Authorization: Bearer [example key]`. Generated in the\n    Archive UI (Settings -> API). Scoped per workspace/agency; must accompany\
  \ the\n    WORKSPACE-ID header.\n  sources: [https://api-docs.archive.com]\n- name: workspaceId\n  type: apiKey\n  in: header\n  parameterName: WORKSPACE-ID\n  description: >-\n    Workspace UUID identifying which workspace the token operates against. Required for\n    workspace-scoped queries; passed as a header, never in the request body.\n  sources: [https://api-docs.archive.com]\n- name: mcpOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization used by the hosted MCP server (app.archive.com/api/v2/mcp).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.archive.com/oauth/authorize\n    tokenUrl: https://app.archive.com/oauth/token\n    registrationUrl: https://app.archive.com/oauth/register\n    codeChallengeMethods: [S256]\n    scopes: [mcp]\n  sources: [https://app.archive.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archive-technologies/refs/heads/main/authentication/archive-technologies-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Creator Marketing
- Influencer Marketing
- Social Listening
- User Generated Content
- E-commerce
- GraphQL
- MCP
---
