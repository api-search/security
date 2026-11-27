---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Den Authentication
name_suffix: Authentication
oauth_flows: []
overview: Den declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Den
provider_slug: den-archi
scheme_count: 3
schemes:
- authorization_url: https://mcp.den.archi/authorize
  bearer_methods:
  - header
  description: Web connectors (Claude, ChatGPT custom connectors) register https://mcp.den.archi/mcp and authenticate with OAuth; the docs say no key is placed in the URL ("주소에 키가 포함되지 않습니다").
  flow: authorizationCode
  issuer: https://mcp.den.archi
  name: oauth2-authorization-code-pkce
  pkce: S256
  registration_url: https://mcp.den.archi/register
  scopes:
  - den.read
  token_endpoint_auth_methods:
  - none
  token_url: https://mcp.den.archi/token
  type: oauth2
- description: 'For clients without connector auth, a personal key issued per channel from the mcp.den.archi dashboard after approval is sent as "Authorization: Bearer {개인키}" (Claude Code, Codex CLI via --bearer-token-env-var, Antigravity mcp_config.json headers, and the Claude Desktop den.mcpb extension).'
  key_issuance: dashboard after beta approval; one key per channel recommended
  name: personal-key-bearer
  scheme: bearer
  type: http
- description: claude.ai web/mobile and ChatGPT developer mode may use https://mcp.den.archi/mcp/{개인키}; the docs warn the key is exposed in the URL during screen sharing.
  in: path
  name: personal-key-in-path
  type: apiKey
slug: den-archi-authentication
source_filename: den-archi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://den.archi/beta.html\n- https://mcp.den.archi/.well-known/oauth-authorization-server\n- https://mcp.den.archi/.well-known/oauth-protected-resource\ndocs: https://den.archi/beta.html\nnote: No OpenAPI is published; the profile is read from the provider's connection guide (beta.html, Korean) and its\n  OAuth discovery documents. Access requires an approved beta application. Authentication/token endpoints were\n  read from metadata only and never called.\nschemes:\n- name: oauth2-authorization-code-pkce\n  type: oauth2\n  flow: authorizationCode\n  description: Web connectors (Claude, ChatGPT custom connectors) register https://mcp.den.archi/mcp and authenticate\n    with OAuth; the docs say no key is placed in the URL (\"주소에 키가 포함되지 않습니다\").\n  issuer: https://mcp.den.archi\n  authorization_url: https://mcp.den.archi/authorize\n  token_url: https://mcp.den.archi/token\n  registration_url: https://mcp.den.archi/register\n\
  \  pkce: S256\n  token_endpoint_auth_methods: [none]\n  scopes: [den.read]\n  bearer_methods: [header]\n- name: personal-key-bearer\n  type: http\n  scheme: bearer\n  description: 'For clients without connector auth, a personal key issued per channel from the mcp.den.archi\n    dashboard after approval is sent as \"Authorization: Bearer {개인키}\" (Claude Code, Codex CLI via\n    --bearer-token-env-var, Antigravity mcp_config.json headers, and the Claude Desktop den.mcpb extension).'\n  key_issuance: dashboard after beta approval; one key per channel recommended\n- name: personal-key-in-path\n  type: apiKey\n  in: path\n  description: claude.ai web/mobile and ChatGPT developer mode may use https://mcp.den.archi/mcp/{개인키}; the docs\n    warn the key is exposed in the URL during screen sharing.\n"
source_yaml_url: https://artifacts.apis.io/den-archi/authentication/den-archi-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Architecture
- Construction
- AEC
- Building Codes
- Standards
- Knowledge Base
- MCP
- AI Agents
- South Korea
---
