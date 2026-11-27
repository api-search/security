---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dibri-ai-openapi-generated.yml
  format: yaml
  label: Dibri API
  slug: dibri-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibri-ai/openapi/_ae-authored/dibri-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dibri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dibri declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dibri
provider_slug: dibri-ai
scheme_count: 2
schemes:
- applies_to:
  - POST /api/v1/agent/query
  - MCP tool ask at https://dibri.ai/mcp
  description: Per-agent token created under Agents -> New agent; "It is shown only once, so store it somewhere safe. Each agent answers from exactly one vault."
  header: 'Authorization: Bearer YOUR_AGENT_TOKEN'
  name: agent-token
  scheme: bearer
  type: http
- applies_to:
  - GET /api/v1/analytics
  - GET /api/v1/analytics/{tool}
  - MCP trust tools at https://dibri.ai/mcp
  description: Read-only analytics key created under API Keys; "keep analytics keys on your own servers and never in a website or widget."
  header: 'Authorization: Bearer dbk_YOUR_KEY'
  name: analytics-key
  prefix: dbk_
  scheme: bearer
  type: http
slug: dibri-ai-authentication
source_filename: dibri-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dibri.ai/developers\ndocs: https://dibri.ai/developers#quickstart\nschemes:\n- name: agent-token\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer YOUR_AGENT_TOKEN'\n  applies_to: [POST /api/v1/agent/query, MCP tool ask at https://dibri.ai/mcp]\n  description: Per-agent token created under Agents -> New agent; \"It is shown only once, so store it somewhere safe. Each agent answers from exactly one vault.\"\n- name: analytics-key\n  type: http\n  scheme: bearer\n  prefix: dbk_\n  header: 'Authorization: Bearer dbk_YOUR_KEY'\n  applies_to: ['GET /api/v1/analytics', 'GET /api/v1/analytics/{tool}', 'MCP trust tools at https://dibri.ai/mcp']\n  description: Read-only analytics key created under API Keys; \"keep analytics keys on your own servers and never in a website or widget.\"\noauth2: false\nnote: No OAuth flows are documented; scopes/ artifact not applicable.\n"
source_yaml_url: https://artifacts.apis.io/dibri-ai/authentication/dibri-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Knowledge Base
- RAG
- Customer Service
- MCP
- REST API
---
