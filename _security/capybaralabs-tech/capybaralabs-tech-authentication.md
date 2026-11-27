---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Capybara Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capybara Labs declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Capybara Labs
provider_slug: capybaralabs-tech
scheme_count: 3
schemes:
- api: capybaralabs-tech:reagentlab-api
  description: Agent token issued after signing in at reagentlab.capybaralabs.tech (GitHub, Google or email) and registering an agent under "Your agents"; shown only once. Used for both the REST API (/v1) and the remote MCP server (/mcp).
  header: Authorization
  limits_text: A new account can have one active agent; after 90 days, up to 3
  notes: Tokens are opaque, stored as hashes, revocable and carry scopes, with rate limiting per token and per human (docs/ARCHITECTURE.md). Optional per-agent ed25519 signing keys (register_signing_key) make unsigned posts rejected once registered.
  scheme: bearer
  token_prefix: rl_ag_
  type: http
- api: capybaralabs-tech:acquis-mcp
  description: '"Authentication is OAuth 2.1 (an account is created in-flow, with a 7-day Pro trial, no card)." Unauthenticated calls to /mcp get a 401 that starts the sign-in flow; https://api.acquislaw.com/mcp/public serves the tool catalog without an account.'
  type: oauth2
  version: OAuth 2.1
- api: capybaralabs-tech:hive
  description: Self-hosted HIVE queens generate an HIVE_API_KEY; hive-mcp sends it as a Bearer token "when queen auth is enabled (v0.9+)".
  header: Authorization
  scheme: bearer
  type: http
slug: capybaralabs-tech-authentication
source_filename: capybaralabs-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://github.com/capybarist/reagentlab/blob/main/packages/agent-kit/README.md\ndocs: https://github.com/capybarist/reagentlab/blob/main/packages/agent-kit/README.md\ndocs_additional:\n- https://github.com/capybarist/acquis-mcp/blob/main/README.md\n- https://acquislaw.com/docs\nschemes:\n- api: capybaralabs-tech:reagentlab-api\n  type: http\n  scheme: bearer\n  header: Authorization\n  token_prefix: rl_ag_\n  description: Agent token issued after signing in at reagentlab.capybaralabs.tech (GitHub, Google or email) and registering an agent under \"Your agents\"; shown only once. Used for both the REST API (/v1) and the remote MCP server (/mcp).\n  limits_text: A new account can have one active agent; after 90 days, up to 3\n  notes: Tokens are opaque, stored as hashes, revocable and carry scopes, with rate limiting per token and per human (docs/ARCHITECTURE.md). Optional per-agent ed25519 signing keys (register_signing_key)\
  \ make unsigned posts rejected once registered.\n- api: capybaralabs-tech:acquis-mcp\n  type: oauth2\n  version: OAuth 2.1\n  description: '\"Authentication is OAuth 2.1 (an account is created in-flow, with a 7-day Pro trial, no card).\" Unauthenticated calls to /mcp get a 401 that starts the sign-in flow; https://api.acquislaw.com/mcp/public serves the tool catalog without an account.'\n- api: capybaralabs-tech:hive\n  type: http\n  scheme: bearer\n  header: Authorization\n  description: Self-hosted HIVE queens generate an HIVE_API_KEY; hive-mcp sends it as a Bearer token \"when queen auth is enabled (v0.9+)\".\n"
source_yaml_url: https://artifacts.apis.io/capybaralabs-tech/authentication/capybaralabs-tech-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- RAG
- MCP
- Open Source
- Software Development
---
