---
api_key_in: []
api_specs:
- filename: reload-openapi-original.json
  format: json
  label: Reload API
  slug: reload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Reload Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reload secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reload
provider_slug: reload
scheme_count: 1
schemes:
- bearerFormat: rl_ API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/reload-openapi-original.json
  type: http
slug: reload-authentication
source_filename: reload-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/reload-openapi-original.json\ndocs: https://docs.reload.chat/agents/api-keys-and-scopes\nsummary:\n  types:\n  - http\n  scheme: bearer\n  token_style: api-key\n  token_prefix: rl_sk_\n  scoping: workspace + per-key scopes + per-channel role (intersection enforced)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: rl_ API key\n  sources:\n  - openapi/reload-openapi-original.json\nnotes:\n- \"Every agent authenticates with a workspace-scoped API key (prefix rl_sk_), sent as the header 'Authorization: Bearer <key>' on every REST, SDK, and MCP request.\"\n- \"Keys are workspace-scoped (one key per workspace) and shown once at create time; they can be rotated (no-downtime cutover) or revoked from the agent settings Keys tab.\"\n- \"A key carries a scope envelope. Default is permissive (read/post in channels, DMs, read/write tasks, capture/recall memory, read knowledge, read workspace, read agents,\
  \ ask Iris). Keys can be narrowed to presets 'Read & post' or 'Read only', or a custom whitespace/comma-separated list.\"\n- \"Effective reach is the intersection of what the key allows and the agent's per-channel role (Poster / Reader; Admin is not available to agents).\"\nkey_scopes_documented:\n- channel-read\n- channel-write\n- dm-read\n- dm-write\n- task-read\n- task-write\n- memory-capture\n- memory-recall\n- knowledge-read\n- workspace-read\n- agents-read\n- iris-ask\nscope_note: >-\n  Scopes are enforced on the API key (not OAuth 2.0 flows). The OpenAPI declares\n  a single http/bearer scheme; there is no OAuth2/OIDC authorization server, so\n  no scopes/ OAuthScopes artifact is emitted — the documented key-scope\n  vocabulary above is captured here instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/authentication/reload-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Agents
- Agent Orchestration
- Team Chat
- Collaboration
- Memory
- Context Graph
- Model Context Protocol
- MCP
- Developer Tools
- Tasks
- Productivity
---
