---
api_key_in: []
auth_types: []
description: 'machine0''s control plane authenticates with OAuth 2.0. Interactive clients (the CLI `machine0 login`, and MCP clients such as Claude Desktop / Claude Code / the claude.ai custom connector) run a browser-based authorization-code flow with PKCE; the MCP server advertises itself as an RFC 9728 OAuth protected resource with RFC 8414 authorization-server metadata and RFC 7591 dynamic client registration. Programmatic/automation access uses a static credential: an API key via the x-api-key header (MCP) or the MACHINE0_API_TOKEN environment variable (CLI). SSH access to VMs is a separate, key-based layer.'
kind: authentication
layout: security
method: searched
name: Machine0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Machine0 declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Machine0
provider_slug: machine0
scheme_count: 4
schemes:
- authorization_endpoint: https://app.machine0.io/api/auth/mcp/authorize
  discovery:
    authorization_server: well-known/machine0-oauth-authorization-server.json
    protected_resource: well-known/machine0-mcp-oauth-protected-resource.json
  flow: authorization_code
  id_token_signing_alg: RS256
  issuer: https://app.machine0.io
  name: machine0 OAuth
  pkce: S256
  registration_endpoint: https://app.machine0.io/api/auth/mcp/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  token_endpoint: https://app.machine0.io/api/auth/mcp/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  used_by:
  - CLI login
  - MCP interactive clients
  userinfo_endpoint: https://app.machine0.io/api/auth/mcp/userinfo
- in: header
  name: x-api-key
  provisioning: Generated from account settings.
  type: apiKey
  used_by:
  - MCP programmatic clients
- in: environment
  name: MACHINE0_API_TOKEN
  type: apiKey
  used_by:
  - CLI automation / non-interactive
- detail: VM shell access uses SSH keys — either a user-registered public key or a server-managed keypair (ssh_key_create_managed) required for remote command execution (ssh_exec). Distinct from control-plane auth.
  name: SSH keypair
  type: ssh
slug: machine0-authentication
source_filename: machine0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://docs.machine0.io/mcp/overview, https://docs.machine0.io/cli/account,\n  and the OAuth discovery documents at\n  https://app.machine0.io/.well-known/oauth-authorization-server\ndescription: >-\n  machine0's control plane authenticates with OAuth 2.0. Interactive clients (the\n  CLI `machine0 login`, and MCP clients such as Claude Desktop / Claude Code / the\n  claude.ai custom connector) run a browser-based authorization-code flow with\n  PKCE; the MCP server advertises itself as an RFC 9728 OAuth protected resource\n  with RFC 8414 authorization-server metadata and RFC 7591 dynamic client\n  registration. Programmatic/automation access uses a static credential: an API\n  key via the x-api-key header (MCP) or the MACHINE0_API_TOKEN environment\n  variable (CLI). SSH access to VMs is a separate, key-based layer.\nschemes:\n  - type: oauth2\n    name: machine0 OAuth\n    flow: authorization_code\n    pkce: S256\n\
  \    issuer: https://app.machine0.io\n    authorization_endpoint: https://app.machine0.io/api/auth/mcp/authorize\n    token_endpoint: https://app.machine0.io/api/auth/mcp/token\n    userinfo_endpoint: https://app.machine0.io/api/auth/mcp/userinfo\n    registration_endpoint: https://app.machine0.io/api/auth/mcp/register\n    scopes: [openid, profile, email, offline_access]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    id_token_signing_alg: RS256\n    used_by: [CLI login, MCP interactive clients]\n    discovery:\n      protected_resource: well-known/machine0-mcp-oauth-protected-resource.json\n      authorization_server: well-known/machine0-oauth-authorization-server.json\n  - type: apiKey\n    name: x-api-key\n    in: header\n    used_by: [MCP programmatic clients]\n    provisioning: Generated from account settings.\n  - type: apiKey\n    name: MACHINE0_API_TOKEN\n    in: environment\n    used_by: [CLI automation / non-interactive]\n  - type: ssh\n\
  \    name: SSH keypair\n    detail: >-\n      VM shell access uses SSH keys — either a user-registered public key or a\n      server-managed keypair (ssh_key_create_managed) required for remote command\n      execution (ssh_exec). Distinct from control-plane auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machine0/refs/heads/main/authentication/machine0-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Cloud
- Infrastructure
- Virtual Machines
- AI Agents
- Developer Tools
- CLI
- MCP
---
