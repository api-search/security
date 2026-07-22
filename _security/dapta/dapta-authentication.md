---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dapta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dapta secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dapta
provider_slug: dapta
scheme_count: 1
schemes:
- in: header
  lifecycle:
    one_active_key_per_workspace: true
    owner_only: true
    recoverable: false
    rotation: revoke current key then mint a new one on the MCP Access tab
    shown_once: true
  name: workspaceApiKey
  notes: Dapta authenticates AI clients to a single workspace with a workspace-scoped API key passed in the x-api-key header. The same key authorizes the hosted MCP server at https://mcp.dapta.ai/mcp. No OpenAPI is published, so this profile is sourced from the developer documentation rather than derived.
  parameter_name: x-api-key
  scope: workspace
  sources:
  - https://docs.dapta.ai/dapta-mcp/setup/connect-codex
  type: apiKey
slug: dapta-authentication
source_filename: dapta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.dapta.ai/dapta-mcp/setup/mint-your-api-key\ndocs: https://docs.dapta.ai/dapta-mcp/key-concepts\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: workspaceApiKey\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    scope: workspace\n    lifecycle:\n      one_active_key_per_workspace: true\n      owner_only: true\n      shown_once: true\n      recoverable: false\n      rotation: revoke current key then mint a new one on the MCP Access tab\n    notes: >-\n      Dapta authenticates AI clients to a single workspace with a workspace-scoped\n      API key passed in the x-api-key header. The same key authorizes the hosted\n      MCP server at https://mcp.dapta.ai/mcp. No OpenAPI is published, so this\n      profile is sourced from the developer documentation rather than derived.\n    sources:\n      - https://docs.dapta.ai/dapta-mcp/setup/connect-codex\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dapta/refs/heads/main/authentication/dapta-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Agents
- Voice AI
- Conversational AI
- Automation
- No-Code
- Model Context Protocol
- Webhooks
- CRM
- SMB
---
