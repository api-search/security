---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: DiagramZu Authentication
name_suffix: Authentication
oauth_flows: []
overview: DiagramZu declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: DiagramZu
provider_slug: diagramzu-ai
scheme_count: 3
schemes:
- applies_to:
  - REST API https://diagramzu.ai/api/spaces/{spaceId}/...
  - MCP https://mcp.diagramzu.ai/mcp
  issuance: Open /app/settings/connections and generate one. Copy it immediately — you won't see it again.
  name: apiToken
  scheme: bearer
  scope_model: A token is scoped either to one workspace or to all the workspaces its owner belongs to, chosen when the token is authorized (per the @diagramzu/mcp README).
  source: https://diagramzu.ai/docs
  token_prefix: dz_live_
  type: http
- applies_to:
  - MCP https://mcp.diagramzu.ai/mcp
  description: '"In Claude, open Settings → Connectors → Add custom connector, paste https://mcp.diagramzu.ai/mcp , and authorize with your DiagramZu account. No API token to copy." Flows, scopes and endpoints are not documented on the docs page.'
  name: claudeConnectorOAuth
  source: https://diagramzu.ai/docs
  type: oauth2
- description: Browser sign-in session; required for share-link minting/revocation, token create/revoke and page delete ("Needs a signed-in session — an API token gets 403").
  name: session
  source: https://diagramzu.ai/docs
  type: cookie-session
slug: diagramzu-ai-authentication
source_filename: diagramzu-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://diagramzu.ai/docs\ndocs: https://diagramzu.ai/docs\nsummary: >-\n  Every REST request and every MCP call carries an `Authorization: Bearer <token>` header holding a DiagramZu API token\n  (prefix dz_live_), minted at /app/settings/connections and shown once. The Claude custom connector instead authorizes\n  with the DiagramZu account through OAuth (no token copied). Some endpoints (minting share links, creating/revoking tokens,\n  deleting pages) need a signed-in browser session; the docs state an API token gets 403 on them.\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  token_prefix: dz_live_\n  applies_to:\n  - 'REST API https://diagramzu.ai/api/spaces/{spaceId}/...'\n  - MCP https://mcp.diagramzu.ai/mcp\n  issuance: \"Open /app/settings/connections and generate one. Copy it immediately — you won't see it again.\"\n  scope_model: A token is scoped either to one workspace or to all the workspaces its\
  \ owner belongs to, chosen when the token\n    is authorized (per the @diagramzu/mcp README).\n  source: https://diagramzu.ai/docs\n- name: claudeConnectorOAuth\n  type: oauth2\n  applies_to:\n  - MCP https://mcp.diagramzu.ai/mcp\n  description: >-\n    \"In Claude, open Settings → Connectors → Add custom connector, paste https://mcp.diagramzu.ai/mcp , and authorize\n    with your DiagramZu account. No API token to copy.\" Flows, scopes and endpoints are not documented on the docs page.\n  source: https://diagramzu.ai/docs\n- name: session\n  type: cookie-session\n  description: Browser sign-in session; required for share-link minting/revocation, token create/revoke and page delete\n    (\"Needs a signed-in session — an API token gets 403\").\n  source: https://diagramzu.ai/docs\n"
source_yaml_url: https://artifacts.apis.io/diagramzu-ai/authentication/diagramzu-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Diagramming
- Mermaid
- MCP
- Developer Tools
- Documentation
- Collaboration
- AI Agents
---
