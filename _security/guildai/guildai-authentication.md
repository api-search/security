---
api_key_in:
- header
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Guildai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Guild.ai secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Guild.ai
provider_slug: guildai
scheme_count: 3
schemes:
- applies_to: Guildcode REST API (session create, events, tasks)
  base_url: https://app.guild.ai/api
  evidence: '"Guildcode uses HTTP Basic Authentication to authorize API requests. Pass the combined credentials string as the authentication parameter (for example, with `curl -u`)." — docs.guild.ai/platform/triggers.md'
  name: guildcode-basic
  scheme: basic
  sources:
  - docs.guild.ai/platform/triggers.md
  type: http
- applies_to: External systems invoking Guild triggers over HTTP
  docs: https://docs.guild.ai/platform/trigger-api-keys.md
  in: header
  name: trigger-api-key
  scope: Each key is scoped to a specific trigger.
  sources:
  - docs.guild.ai/platform/trigger-api-keys.md
  type: apiKey
- applies_to: Guild CLI (`guild auth login` opens the browser to sign in at app.guild.ai)
  flow: authorizationCode
  name: cli-oauth
  sources:
  - docs.guild.ai/cli/getting-started.md
  type: oauth2
slug: guildai-authentication
source_filename: guildai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.guild.ai/platform/triggers.md\ndocs: https://docs.guild.ai/platform/trigger-api-keys.md\nsummary:\n  types: [http, apiKey, oauth2]\n  http_schemes: [basic]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Guild has no public OpenAPI spec; this profile is searched from the docs. The\n    Guildcode REST API (base https://app.guild.ai/api) uses HTTP Basic Authentication;\n    programmatic trigger invocation uses per-trigger API keys; the CLI authenticates\n    via browser-based OAuth (`guild auth login`). Enterprise adds SSO, SCIM, and RBAC.\nschemes:\n  - name: guildcode-basic\n    type: http\n    scheme: basic\n    applies_to: Guildcode REST API (session create, events, tasks)\n    base_url: https://app.guild.ai/api\n    evidence: >-\n      \"Guildcode uses HTTP Basic Authentication to authorize API requests. Pass the\n      combined credentials string as the authentication parameter\
  \ (for example, with\n      `curl -u`).\" — docs.guild.ai/platform/triggers.md\n    sources: [docs.guild.ai/platform/triggers.md]\n  - name: trigger-api-key\n    type: apiKey\n    in: header\n    applies_to: External systems invoking Guild triggers over HTTP\n    scope: Each key is scoped to a specific trigger.\n    docs: https://docs.guild.ai/platform/trigger-api-keys.md\n    sources: [docs.guild.ai/platform/trigger-api-keys.md]\n  - name: cli-oauth\n    type: oauth2\n    flow: authorizationCode\n    applies_to: Guild CLI (`guild auth login` opens the browser to sign in at app.guild.ai)\n    sources: [docs.guild.ai/cli/getting-started.md]\nenterprise:\n  sso: true\n  scim: true\n  rbac: true\n  source: https://guild.ai/solutions/enterprise\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guildai/refs/heads/main/authentication/guildai-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Company
- Ai
- AI Agents
- Agent Control Plane
- Agent Runtime
- Developer Tools
- MCP
- LLM
- Agent Governance
- SDK
- CLI
---
