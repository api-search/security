---
anonymous_access: false
api_key_in: []
api_specs:
- filename: comment-io-run-api-openapi.yml
  format: yaml
  label: Comment.io Run API
  slug: comment-io-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comment-io/openapi/comment-io-run-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Comment.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comment.io secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Comment.io
provider_slug: comment-io
scheme_count: 2
schemes:
- bearerFormat: commentio_ followed by 64 hex digits
  description: Created by a workspace member in Settings, under Agents, or by an approved AgentID sign-in (https://comment.io/auth/agentid?workspace=WORKSPACE&agent=AGENT) where offered. The token does not expire; rolling it in Settings stops the old one at once; it also stops when the agent is disconnected, when the human who made it leaves the workspace, or when the workspace is deleted.
  endpoint: https://comment.io/api/run
  name: apiToken
  scheme: bearer
  sources:
  - openapi/comment-io-openapi.yml
  - https://comment.io/llms/http-api.md
  - https://comment.io/auth.md
  type: http
- client_registration:
  - Client ID Metadata Document (client_id is an HTTPS URL)
  - Dynamic client registration (RFC 7591) at https://comment.io/oauth/register
  - Any other opaque client_id of 1 to 255 characters
  description: OAuth 2.1 authorization code. The docs state "there are no scopes"; a grant is for one agent in one workspace, at one MCP server. The WorkOS agent-registration methods (identity_endpoint, ID-JAG, service_auth, anonymous registration) are explicitly not offered.
  discovery:
    authorization_server_metadata: https://comment.io/.well-known/oauth-authorization-server
    protected_resource_metadata:
    - https://comment.io/.well-known/oauth-protected-resource/mcp
    - https://comment.io/.well-known/oauth-protected-resource/mcp/tools
    - https://comment.io/.well-known/oauth-protected-resource/api/run
  endpoint:
  - https://comment.io/mcp
  - https://comment.io/mcp/tools
  flows:
    authorizationCode:
      authorizationUrl: https://comment.io/oauth/authorize
      refreshUrl: https://comment.io/oauth/token
      scopes: {}
      tokenUrl: https://comment.io/oauth/token
  name: mcpOAuth
  pkce: S256 required for public clients; optional for configured confidential clients
  resource_indicator: resource parameter must be exactly https://comment.io/mcp or https://comment.io/mcp/tools (default /mcp)
  sources:
  - https://comment.io/auth.md
  - https://comment.io/llms/mcp.md
  token_lifetime: 'expires_in: 7776000 in the documented example; each refresh issues a new refresh token and the old one stops working'
  type: oauth2
slug: comment-io-authentication
source_filename: comment-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comment.io/auth.md\ndocs: https://comment.io/auth.md\nsummary:\n  types:\n  - http\n  - oauth2\n  note: Three agent endpoints, each with its own credential. /api/run takes a bearer API token; /mcp and /mcp/tools take OAuth 2.1 access tokens. A token works only at its own endpoint (except a Microsoft Copilot grant for /mcp also works at /mcp/tools). No self-service registration; a human member of the workspace grants every credential.\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  bearerFormat: commentio_ followed by 64 hex digits\n  endpoint: https://comment.io/api/run\n  description: Created by a workspace member in Settings, under Agents, or by an approved AgentID sign-in (https://comment.io/auth/agentid?workspace=WORKSPACE&agent=AGENT) where offered. The token does not expire; rolling it in Settings stops the old one at once; it also stops when the agent is disconnected, when the human who made it\
  \ leaves the workspace, or when the workspace is deleted.\n  sources:\n  - openapi/comment-io-openapi.yml\n  - https://comment.io/llms/http-api.md\n  - https://comment.io/auth.md\n- name: mcpOAuth\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://comment.io/oauth/authorize\n      tokenUrl: https://comment.io/oauth/token\n      refreshUrl: https://comment.io/oauth/token\n      scopes: {}\n  endpoint:\n  - https://comment.io/mcp\n  - https://comment.io/mcp/tools\n  pkce: S256 required for public clients; optional for configured confidential clients\n  resource_indicator: resource parameter must be exactly https://comment.io/mcp or https://comment.io/mcp/tools (default /mcp)\n  client_registration:\n  - Client ID Metadata Document (client_id is an HTTPS URL)\n  - Dynamic client registration (RFC 7591) at https://comment.io/oauth/register\n  - Any other opaque client_id of 1 to 255 characters\n  discovery:\n    protected_resource_metadata:\n    - https://comment.io/.well-known/oauth-protected-resource/mcp\n\
  \    - https://comment.io/.well-known/oauth-protected-resource/mcp/tools\n    - https://comment.io/.well-known/oauth-protected-resource/api/run\n    authorization_server_metadata: https://comment.io/.well-known/oauth-authorization-server\n  token_lifetime: 'expires_in: 7776000 in the documented example; each refresh issues a new refresh token and the old one stops working'\n  description: OAuth 2.1 authorization code. The docs state \"there are no scopes\"; a grant is for one agent in one workspace, at one MCP server. The WorkOS agent-registration methods (identity_endpoint, ID-JAG, service_auth, anonymous registration) are explicitly not offered.\n  sources:\n  - https://comment.io/auth.md\n  - https://comment.io/llms/mcp.md\n"
source_yaml_url: https://artifacts.apis.io/comment-io/authentication/comment-io-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- AI Agents
- Collaboration
- Documents
- Markdown
- MCP
- Knowledge Management
- Workspace
---
