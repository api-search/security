---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agentspodium-com-openapi.yml
  format: yaml
  label: AgentsPodium Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentspodium-com/refs/heads/main/openapi/agentspodium-com-openapi.yml
auth_types:
- http
description: 'One bearer scheme with two credential kinds. An API key (ak_live_...) is created by a signed-in person on https://agentspodium.com/account ("API keys for agents"), carries the same rights as that person''s sign-in, never expires, and can be revoked from the same page. A session token comes from a passwordless e-mail code (POST /auth/request -> 202 always, six-digit code valid 10 minutes -> POST /auth/verify) and lives 30 days. Both are sent as "Authorization: Bearer <token>" on every authenticated endpoint. Key management itself (POST /keys, DELETE /keys/{id}) is refused to a key (403) and reserved for the person''s session.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentspodium Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentsPodium secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgentsPodium
provider_slug: agentspodium-com
scheme_count: 1
schemes:
- applied: 'globally (security: [{bearerAuth: []}]); overridden to none on the 11 public operations'
  description: An API key `ak_live_…` created on the account page, or a session token from /auth/verify.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agentspodium-com-openapi.yml
  type: http
slug: agentspodium-com-authentication
source_filename: agentspodium-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/agentspodium-com-openapi.yml\ndocs: https://hosting.defispace.com/docs/auth.html\ndocs_markdown: https://hosting.defispace.com/docs/auth.md\nsummary:\n  types: [http]\n  schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  credential_kinds: [API key (ak_live_), session token (e-mail code)]\n  public_operations: 11\n  authenticated_operations: 41\ndescription: >-\n  One bearer scheme with two credential kinds. An API key (ak_live_...) is created by a signed-in person on\n  https://agentspodium.com/account (\"API keys for agents\"), carries the same rights as that person's sign-in, never\n  expires, and can be revoked from the same page. A session token comes from a passwordless e-mail code\n  (POST /auth/request -> 202 always, six-digit code valid 10 minutes -> POST /auth/verify) and lives 30 days. Both are\n  sent as \"Authorization: Bearer <token>\" on every authenticated endpoint. Key management itself\
  \ (POST /keys,\n  DELETE /keys/{id}) is refused to a key (403) and reserved for the person's session.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An API key `ak_live_…` created on the account page, or a session token from /auth/verify.\n  applied: 'globally (security: [{bearerAuth: []}]); overridden to none on the 11 public operations'\n  sources: [openapi/agentspodium-com-openapi.yml]\ncredentials:\n- kind: API key\n  prefix: ak_live_\n  issued_by: a signed-in person at https://agentspodium.com/account (\"API keys for agents\")\n  lifetime: does not expire\n  revocation: from the account page; a revoked key answers 401 \"Invalid or revoked API key\" everywhere\n  restrictions: cannot create or revoke keys (POST /keys, DELETE /keys/{id} answer 403)\n  recommended_for: agents\n- kind: session token\n  flow: 'POST /auth/request {\"email\"} (202 always — never reveals whether the address exists; 10 per 10 minutes per IP) -> six-digit code by e-mail, valid\
  \ 10 minutes -> POST /auth/verify {\"email\",\"code\"} -> {\"token\",\"user\":{\"id\":\"usr_…\",\"email\"}}'\n  lifetime: 30 days\n  recommended_for: people, and agents that can read the mailbox (IMAP or a mail API)\ngateway_headers:\n  note: The MCP gateway (mcp.agentspodium.com) and A2A gateway (a2a.agentspodium.com) forward the same credential to the account API and additionally accept an x-api-key header or an apiKey query parameter (from the gateway's own 401 body and developer-ai.txt). The A2A agent card declares the same scheme as securitySchemes.bearerAuth.\npublic_operations:\n- GET /engines\n- GET /tiers\n- GET /personas\n- GET /personas/{id}\n- GET /tools\n- GET /models\n- GET /llm-providers\n- GET /status\n- GET /a2a-catalog\n- POST /auth/request\n- POST /auth/verify\nfailure_modes:\n- {status: 401, code: UNAUTHORIZED, when: 'no bearer, expired session, revoked key', observed: '{\"error\":\"UNAUTHORIZED\",\"message\":\"Authentication required\"} on GET /api/agents without a\
  \ token (2026-09-19)'}\n- {status: 403, code: FORBIDDEN, when: 'a key managing keys; someone else''s agent'}\n- {status: 429, when: '/auth/request rate limit exceeded'}\noidc_note: >-\n  https://agentspodium.com/.well-known/openid-configuration advertises an OpenID Provider at https://app.agentspodium.com\n  (authorization_code + PKCE, RS256, scopes openid profile email). This is the account identity provider that signs pod\n  owners into their engine dashboards (the \"sso\" capability on GET /api/engines), not an OAuth flow for the account API,\n  MCP server or A2A agent — none of which publishes OAuth metadata or accepts anything but the bearer key/session token.\n  Saved at well-known/agentspodium-com-openid-configuration.json.\nscopes: none — the key inherits the full rights of the person who created it; there is no scoped or read-only key\nx-evidence:\n  fetched: '2026-09-19'\n  probes:\n  - {url: 'https://hosting.defispace.com/docs/auth.md', http_status: 200}\n  - {url: 'https://agentspodium.com/api/agents',\
  \ http_status: 401, note: unauthenticated}\n  - {url: 'https://agentspodium.com/api/tiers', http_status: 200, note: public}\n  - {url: 'https://mcp.agentspodium.com/mcp', method: POST, body: 'tools/call list_instances (no key)', http_status: 200, note: 'UNAUTHORIZED body naming Authorization Bearer, x-api-key and apiKey'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentspodium-com/refs/heads/main/authentication/agentspodium-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Agent Hosting
- MCP
- A2A
- agent-native
- Hosting
- Webhook
- Personal Assistants
- Company
---
