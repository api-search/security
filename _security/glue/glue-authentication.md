---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Glue Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Glue secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Glue
provider_slug: glue
scheme_count: 2
schemes:
- context: public GraphQL API (https://api.gluegroups.com/public/graphql)
  flow: clientCredentials
  name: GraphQLOAuth2ClientCredentials
  notes: 'Apps register an OAuth Application, then exchange client credentials for a workspace-scoped access token (subject = workspace ID). Token is passed as Authorization: Bearer <ACCESS_TOKEN> to the GraphQL endpoint. No refresh token.

    '
  parameters:
  - grant_type
  - client_id
  - client_secret
  - subject
  - redirect_uri
  refresh_token: false
  scopes:
  - workspaces:read
  - threads:read
  - groups:read
  - threads.messages:write
  token_endpoint: https://api.gluegroups.com/oauth/token
  token_format: opaque bearer
  type: oauth2
- authorization_endpoint: https://api.glue.ai/oauth/authorize
  context: hosted MCP server (https://mcp.glue.ai/mcp, issuer https://api.glue.ai)
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: MCPOAuth2AuthorizationCode
  pkce:
  - S256
  registration_endpoint: https://api.glue.ai/oauth/register
  scopes:
  - mcp:read
  - mcp:write
  source: https://api.glue.ai/.well-known/oauth-authorization-server
  token_endpoint: https://api.glue.ai/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: glue-authentication
source_filename: glue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.glue.ai/developers/authentication/oauth-2-0-authentication.md\ndocs: https://docs.glue.ai/developers/authentication/oauth-2-0-authentication.md\nsummary:\n  types: [oauth2]\n  bearer: true\n  oauth2_flows: [clientCredentials, authorizationCode]\nschemes:\n  - name: GraphQLOAuth2ClientCredentials\n    type: oauth2\n    context: public GraphQL API (https://api.gluegroups.com/public/graphql)\n    flow: clientCredentials\n    token_endpoint: https://api.gluegroups.com/oauth/token\n    token_format: opaque bearer\n    refresh_token: false\n    parameters: [grant_type, client_id, client_secret, subject, redirect_uri]\n    notes: >\n      Apps register an OAuth Application, then exchange client credentials for a\n      workspace-scoped access token (subject = workspace ID). Token is passed as\n      Authorization: Bearer <ACCESS_TOKEN> to the GraphQL endpoint. No refresh token.\n    scopes: [workspaces:read, threads:read,\
  \ groups:read, threads.messages:write]\n  - name: MCPOAuth2AuthorizationCode\n    type: oauth2\n    context: hosted MCP server (https://mcp.glue.ai/mcp, issuer https://api.glue.ai)\n    flow: authorizationCode\n    authorization_endpoint: https://api.glue.ai/oauth/authorize\n    token_endpoint: https://api.glue.ai/oauth/token\n    registration_endpoint: https://api.glue.ai/oauth/register\n    dynamic_client_registration: true       # RFC 7591\n    pkce: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none]\n    scopes: [mcp:read, mcp:write]\n    source: https://api.glue.ai/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glue/refs/heads/main/authentication/glue-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- SaaS
- Team Communication
- Messaging
- Collaboration
- GraphQL
- Webhooks
- MCP
- Productivity
- AI Agents
---
