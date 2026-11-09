---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Manifest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Manifest declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Manifest
provider_slug: manifest
scheme_count: 3
schemes:
- applies_to: LLM gateway proxy (/v1/chat/completions, /v1/responses, /v1/messages, /v1/models)
  errors:
  - M001
  - M002
  - M003
  - M004
  - M005
  format: 'Authorization: Bearer mnfst_<key>; keys always start with mnfst_'
  issuance: Generated from the dashboard Harnesses page (or the CLI/MCP agent create and rotate-key tools)
  name: harnessKey
  scheme: bearer
  type: http
- applies_to: Remote MCP management server (https://app.manifest.build/api/v1/mcp)
  description: OAuth 2.1 with authorization-server discovery and browser consent; short-lived revocable access tokens
  name: mcpOAuth
  scopes:
  - mcp:read
  - mcp:write
  - offline_access
  type: oauth2
- applies_to: mnfst CLI
  description: mnfst login opens the dashboard; on approval the CLI receives a token
  name: cliLogin
  type: browser-approval
slug: manifest-authentication
source_filename: manifest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://manifest.build/llm-gateway/docs/reference/api\n- https://manifest.build/llm-gateway/docs/reference/headers\n- https://manifest.build/llm-gateway/docs/integrations/mcp\ndocs: https://manifest.build/llm-gateway/docs/reference/api\ndocs_pages:\n- https://manifest.build/llm-gateway/docs/reference/api\n- https://manifest.build/llm-gateway/docs/reference/headers\n- https://manifest.build/llm-gateway/docs/integrations/mcp\nschemes:\n- name: harnessKey\n  type: http\n  scheme: bearer\n  applies_to: LLM gateway proxy (/v1/chat/completions, /v1/responses, /v1/messages, /v1/models)\n  format: 'Authorization: Bearer mnfst_<key>; keys always start with mnfst_'\n  issuance: Generated from the dashboard Harnesses page (or the CLI/MCP agent create and rotate-key tools)\n  errors: [M001, M002, M003, M004, M005]\n- name: mcpOAuth\n  type: oauth2\n  applies_to: Remote MCP management server (https://app.manifest.build/api/v1/mcp)\n\
  \  description: OAuth 2.1 with authorization-server discovery and browser consent; short-lived revocable access tokens\n  scopes: [mcp:read, mcp:write, offline_access]\n- name: cliLogin\n  type: browser-approval\n  applies_to: mnfst CLI\n  description: mnfst login opens the dashboard; on approval the CLI receives a token\n"
source_yaml_url: https://artifacts.apis.io/manifest/authentication/manifest-authentication.yml
summary_line: 3 schemes
tags:
- Company
- LLM Gateway
- AI Agents
- Artificial Intelligence
- Open Source
- Observability
- OpenAI-Compatible
- Self-Hosted
---
