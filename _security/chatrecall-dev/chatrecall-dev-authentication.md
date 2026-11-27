---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: chat-recall Authentication
name_suffix: Authentication
oauth_flows: []
overview: chat-recall declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: chat-recall
provider_slug: chatrecall-dev
scheme_count: 2
schemes:
- applies_to: https://chatrecall.dev/mcp
  authorization_endpoint: https://chatrecall.dev/api/auth/oauth2/authorize
  authorization_server: https://chatrecall.dev/api/auth
  bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  docs_text: An assistant that cannot run the chat-recall CLI, such as claude.ai, ChatGPT or a browser IDE, connects to the remote MCP endpoint of your server. It signs in with OAuth and then uses the same tools as the local MCP server.
  dpop_signing_alg_values_supported:
  - EdDSA
  - ES256
  - ES512
  - PS256
  - RS256
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  metadata: https://chatrecall.dev/.well-known/oauth-authorization-server
  name: mcp-oauth2
  registration_endpoint: https://chatrecall.dev/api/auth/oauth2/register
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  token_endpoint: https://chatrecall.dev/api/auth/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  type: oauth2
- applies_to: chat-recall CLI to a hosted or self-hosted server
  description: Machines connect with `chat-recall login <server-url>`; a self-hosted server is bootstrapped with an ADMIN_KEY in .env (self-hosting page). The credential format the CLI stores is not documented.
  name: cli-server-login
  type: other
slug: chatrecall-dev-authentication
source_filename: chatrecall-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chatrecall.dev/.well-known/oauth-protected-resource\ndocs: https://github.com/munhq/chat-recall/blob/main/docs/CONNECTORS.md\nname: chat-recall authentication\nschemes:\n- name: mcp-oauth2\n  type: oauth2\n  applies_to: https://chatrecall.dev/mcp\n  bearer_methods_supported: [header]\n  dpop_signing_alg_values_supported: [EdDSA, ES256, ES512, PS256, RS256]\n  authorization_server: https://chatrecall.dev/api/auth\n  metadata: https://chatrecall.dev/.well-known/oauth-authorization-server\n  authorization_endpoint: https://chatrecall.dev/api/auth/oauth2/authorize\n  token_endpoint: https://chatrecall.dev/api/auth/oauth2/token\n  registration_endpoint: https://chatrecall.dev/api/auth/oauth2/register\n  grant_types_supported: [authorization_code, client_credentials, refresh_token]\n  token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post, private_key_jwt]\n  client_id_metadata_document_supported:\
  \ true\n  scopes_supported: [openid, profile, email, offline_access]\n  docs_text: An assistant that cannot run the chat-recall CLI, such as claude.ai, ChatGPT or a browser IDE, connects to the remote MCP endpoint of your server. It signs in with OAuth and then uses the same tools as the local MCP server.\n- name: cli-server-login\n  type: other\n  applies_to: chat-recall CLI to a hosted or self-hosted server\n  description: Machines connect with `chat-recall login <server-url>`; a self-hosted server is bootstrapped with an ADMIN_KEY in .env (self-hosting page). The credential format the CLI stores is not documented.\nnote: Read from published well-known discovery documents (GET only) and the docs; no auth endpoint was called. A probe of https://chatrecall.dev/mcp returned 401 (pre-flight). Self-hosted servers expose the OAuth-backed endpoint only with AUTH_PROVIDER=better-auth.\n"
source_yaml_url: https://artifacts.apis.io/chatrecall-dev/authentication/chatrecall-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Coding Assistants
- Developer Tools
- MCP
- Memory
- Search
- Secret Scanning
- Self-Hosted
- Open Source
---
