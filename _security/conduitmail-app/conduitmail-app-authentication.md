---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Conduit Mail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conduit Mail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Conduit Mail
provider_slug: conduitmail-app
scheme_count: 1
schemes:
- applies_to: https://connect.conduitmail.app/mcp
  bearer_methods:
  - header
  description: OAuth 2.1 authorization code flow with PKCE, browser sign-in to Conduit; "There's no API key to copy or paste." Bearer token sent in the Authorization header.
  discovery:
    authorization_server_metadata: https://connect.conduitmail.app/.well-known/oauth-authorization-server
    protected_resource_metadata: https://connect.conduitmail.app/.well-known/oauth-protected-resource
  dynamic_client_registration: https://connect.conduitmail.app/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://connect.conduitmail.app/oauth/authorize
      refreshUrl: https://connect.conduitmail.app/oauth/token
      scopes:
        email:read: Read and search mail, attachments up to 5 MB, list folders and accounts
        email:write: Organize, draft, reply, send (when enabled) and block senders
        notes:manage: Create and edit notes
        rules:manage: Create, pause and delete automation rules
      tokenUrl: https://connect.conduitmail.app/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: oauth2
  pkce: S256
  revocation_endpoint: https://connect.conduitmail.app/oauth/revoke
  token_endpoint_auth_methods:
  - none
  type: oauth2
  unauthenticated_response: 401 invalid_token (missing bearer token), per the apis.yml MCPServer pointer
slug: conduitmail-app-authentication
source_filename: conduitmail-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://conduitmail.app/agents\ndocs: https://conduitmail.app/agents\nname: Conduit Mail authentication\nnote: No OpenAPI is published. The only programmatic surface is the hosted MCP server; its auth profile is read from the /agents page and the OAuth discovery documents (GET, HTTP 200 each, 2026-11-04). Token, registration and authorize endpoints were NOT called.\nschemes:\n- name: oauth2\n  type: oauth2\n  description: OAuth 2.1 authorization code flow with PKCE, browser sign-in to Conduit; \"There's no API key to copy or paste.\" Bearer token sent in the Authorization header.\n  applies_to: https://connect.conduitmail.app/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://connect.conduitmail.app/oauth/authorize\n      tokenUrl: https://connect.conduitmail.app/oauth/token\n      refreshUrl: https://connect.conduitmail.app/oauth/token\n      scopes:\n        email:read: Read and search mail, attachments\
  \ up to 5 MB, list folders and accounts\n        email:write: Organize, draft, reply, send (when enabled) and block senders\n        rules:manage: Create, pause and delete automation rules\n        notes:manage: Create and edit notes\n  pkce: S256\n  token_endpoint_auth_methods: [none]\n  grant_types: [authorization_code, refresh_token]\n  dynamic_client_registration: https://connect.conduitmail.app/oauth/register\n  revocation_endpoint: https://connect.conduitmail.app/oauth/revoke\n  bearer_methods: [header]\n  discovery:\n    protected_resource_metadata: https://connect.conduitmail.app/.well-known/oauth-protected-resource\n    authorization_server_metadata: https://connect.conduitmail.app/.well-known/oauth-authorization-server\n  unauthenticated_response: 401 invalid_token (missing bearer token), per the apis.yml MCPServer pointer\nrevocation_ui: Settings › Integrations › Connected apps › Revoke. The agent's next call fails.\n"
source_yaml_url: https://artifacts.apis.io/conduitmail-app/authentication/conduitmail-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- Email Client
- Artificial Intelligence
- MCP
- AI Agents
- Productivity
- Automation
---
