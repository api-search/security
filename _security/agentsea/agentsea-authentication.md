---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Agentsea Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentSea declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgentSea
provider_slug: agentsea
scheme_count: 2
schemes:
- applies_to: applications built on the AgentSea NestJS/REST surface
  docs: https://www.agentsea.dev/docs/multi-tenancy/
  expiry: per-key expiresAt is supported (docs example sets a 1-year expiry)
  id: tenant-api-key
  in: unspecified
  issued_by: the self-hoster, via TenantManager.generateApiKey()
  scoped: true
  scopes:
  - agents:read
  - agents:write
  - conversations:read
  scopes_note: 'These three are the scopes shown in the published multi-tenancy example. The scope vocabulary is application-defined - AgentSea does not publish a closed scope reference, so no scopes/ artifact is emitted. This is API-key scoping, not OAuth: no oauth2 flow, no authorization server, no /.well-known/oauth-authorization-server (probed, 404).'
  storage: SHA256-hashed at rest; plaintext returned once at generation and never shown again
  type: apiKey
  verification: TenantManager.verifyApiKey(key) resolves the key to a tenantId
- applies_to: outbound calls the framework makes to LLM, voice and tool providers
  docs: https://www.agentsea.dev/docs/providers/
  examples:
  - ANTHROPIC_API_KEY
  - OPENAI_API_KEY
  - FIGMA_ACCESS_TOKEN
  - N8N_API_KEY
  - GITHUB_TOKEN (when wiring the official MCP GitHub server)
  id: provider-credentials
  in: environment variable
  note: These are the consumer's own credentials with third parties. AgentSea never brokers or proxies them; the CLI stores them in the OS config directory (~/Library/Preferences/agentsea-cli, ~/.config/agentsea-cli, %APPDATA%/agentsea-cli).
  type: apiKey
slug: agentsea-authentication
source_filename: agentsea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-24'\nmethod: searched\nsource: >-\n  https://www.agentsea.dev/docs/multi-tenancy/, https://www.agentsea.dev/api/,\n  https://www.agentsea.dev/docs/gateway/, https://www.agentsea.dev/docs/cli/\ndocs: https://www.agentsea.dev/docs/multi-tenancy/\nnote: >-\n  AgentSea has no vendor-operated API and therefore issues no credentials of its own. There is no\n  signup, no console, and no account. Authentication in AgentSea is a capability the framework\n  gives the SELF-HOSTER: a multi-tenancy layer that mints and verifies scoped, SHA256-hashed API\n  keys for the tenants of an application you run. Separately, the framework consumes third-party\n  LLM/tool provider credentials (Anthropic, OpenAI, Google, Figma, n8n, ...) read from environment\n  variables. This artifact was derived from the published documentation, not from an OpenAPI - no\n  machine-readable spec with securitySchemes is published.\nvendor_credentials: none\naccount_required: false\nschemes:\n-\
  \ id: tenant-api-key\n  type: apiKey\n  in: unspecified\n  applies_to: applications built on the AgentSea NestJS/REST surface\n  issued_by: the self-hoster, via TenantManager.generateApiKey()\n  storage: SHA256-hashed at rest; plaintext returned once at generation and never shown again\n  verification: TenantManager.verifyApiKey(key) resolves the key to a tenantId\n  expiry: per-key expiresAt is supported (docs example sets a 1-year expiry)\n  scoped: true\n  scopes:\n  - agents:read\n  - agents:write\n  - conversations:read\n  scopes_note: >-\n    These three are the scopes shown in the published multi-tenancy example. The scope vocabulary is\n    application-defined - AgentSea does not publish a closed scope reference, so no scopes/ artifact\n    is emitted. This is API-key scoping, not OAuth: no oauth2 flow, no authorization server, no\n    /.well-known/oauth-authorization-server (probed, 404).\n  docs: https://www.agentsea.dev/docs/multi-tenancy/\n- id: provider-credentials\n  type:\
  \ apiKey\n  in: environment variable\n  applies_to: outbound calls the framework makes to LLM, voice and tool providers\n  examples:\n  - ANTHROPIC_API_KEY\n  - OPENAI_API_KEY\n  - FIGMA_ACCESS_TOKEN\n  - N8N_API_KEY\n  - GITHUB_TOKEN (when wiring the official MCP GitHub server)\n  note: >-\n    These are the consumer's own credentials with third parties. AgentSea never brokers or proxies\n    them; the CLI stores them in the OS config directory (~/Library/Preferences/agentsea-cli,\n    ~/.config/agentsea-cli, %APPDATA%/agentsea-cli).\n  docs: https://www.agentsea.dev/docs/providers/\nunauthenticated_by_default: >-\n  The documented /agents REST endpoints and the OpenAI-compatible POST /v1/chat/completions gateway\n  endpoint ship with no authentication of their own. The NestJS guide's production checklist tells\n  the operator to \"implement authentication and authorization guards\" - auth is the deployer's\n  responsibility, not a built-in default.\ntenant_model:\n  isolation: complete\
  \ data separation between tenants; tenant-scoped conversation history and memory stores\n  statuses:\n  - ACTIVE\n  - SUSPENDED\n  - INACTIVE\n  settings:\n  - maxAgents\n  - maxConversations\n  - rateLimit\n  - dataRetentionDays\n  - allowedProviders\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentsea/refs/heads/main/authentication/agentsea-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Orchestration
- Large Language Models
- Model Context Protocol
- Agentic Commerce
- Open Source
- Developer Tools
- SDKs
- TypeScript
- Elixir
- Voice
---
