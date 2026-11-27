---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chief Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chief declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chief
provider_slug: chiefisnext-com
scheme_count: 2
schemes:
- applies_to: https://mcp.chiefisnext.com/mcp
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  description: Users connect an assistant (Claude, Codex, Claude Code, ChatGPT, Cursor), sign in to Chief and select which projects the assistant may access on a consent screen.
  discovery:
    authorization_server_metadata: https://chiefisnext.com/.well-known/oauth-authorization-server
    protected_resource_metadata: https://mcp.chiefisnext.com/.well-known/oauth-protected-resource
  dynamic_client_registration: https://chiefisnext.com/oauth/register
  evidence:
  - http_status: 200
    url: https://mcp.chiefisnext.com/.well-known/oauth-protected-resource
  - http_status: 200
    url: https://chiefisnext.com/.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorizationUrl: https://chiefisnext.com/oauth/authorize
      refreshUrl: https://chiefisnext.com/oauth/token
      scopes:
      - projects:read
      - milestones:read
      - summaries:read
      - manager_tasks:read
      - milestones:propose
      - manager_tasks:write
      tokenUrl: https://chiefisnext.com/oauth/token
  name: chief-oauth
  pkce: S256
  revocation_docs: Open Settings → Connected apps to inspect or revoke a connection. Revocation takes effect on the assistant's next request.
  revocation_endpoint: https://chiefisnext.com/oauth/revoke
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- applies_to: chief-relay (local relay binary)
  description: 'Relay auth: Device code flow — no static API keys stored on your machine. The relay opens a browser verification URL; the user compares the code and selects Approve Device.'
  name: relay-device-code
  source: https://chiefisnext.com/security
  type: device_code
slug: chiefisnext-com-authentication
source_filename: chiefisnext-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chiefisnext.com/docs/mcp\ndocs: https://chiefisnext.com/docs/mcp\nname: Chief authentication\nnote: Chief publishes no REST/OpenAPI contract. Its only public programmatic surface is the remote MCP server at https://mcp.chiefisnext.com/mcp, protected by OAuth 2.0. Values below come from the docs and from the published discovery documents (GET only); no token, login or registration endpoint was called.\nschemes:\n- name: chief-oauth\n  type: oauth2\n  applies_to: https://mcp.chiefisnext.com/mcp\n  description: Users connect an assistant (Claude, Codex, Claude Code, ChatGPT, Cursor), sign in to Chief and select which projects the assistant may access on a consent screen.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://chiefisnext.com/oauth/authorize\n      tokenUrl: https://chiefisnext.com/oauth/token\n      refreshUrl: https://chiefisnext.com/oauth/token\n      scopes:\n      - projects:read\n     \
  \ - milestones:read\n      - summaries:read\n      - manager_tasks:read\n      - milestones:propose\n      - manager_tasks:write\n  pkce: S256\n  dynamic_client_registration: https://chiefisnext.com/oauth/register\n  client_id_metadata_document_supported: true\n  revocation_endpoint: https://chiefisnext.com/oauth/revoke\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  bearer_methods: [header]\n  discovery:\n    protected_resource_metadata: https://mcp.chiefisnext.com/.well-known/oauth-protected-resource\n    authorization_server_metadata: https://chiefisnext.com/.well-known/oauth-authorization-server\n  evidence:\n  - url: https://mcp.chiefisnext.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://chiefisnext.com/.well-known/oauth-authorization-server\n    http_status: 200\n  revocation_docs: \"Open Settings → Connected apps to inspect or revoke a connection. Revocation takes effect on the assistant's next request.\"\n- name:\
  \ relay-device-code\n  type: device_code\n  applies_to: chief-relay (local relay binary)\n  description: \"Relay auth: Device code flow — no static API keys stored on your machine. The relay opens a browser verification URL; the user compares the code and selects Approve Device.\"\n  source: https://chiefisnext.com/security\n"
source_yaml_url: https://artifacts.apis.io/chiefisnext-com/authentication/chiefisnext-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Agents
- Agent Management
- Coding Agents
- Developer Tools
- MCP
- Project Management
---
