---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: live-direct-marketing-online-ldm-v3-openapi.json
  format: json
  label: LDM v3 API
  slug: ldm-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-direct-marketing-online/refs/heads/main/openapi/live-direct-marketing-online-ldm-v3-openapi.json
- filename: live-direct-marketing-online-inbox-check-openapi.json
  format: json
  label: Inbox Check API
  slug: inbox-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-direct-marketing-online/refs/heads/main/openapi/live-direct-marketing-online-inbox-check-openapi.json
auth_types:
- http bearer
- apiKey (header)
- cookie session
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Live Direct Marketing Online Authentication
name_suffix: Authentication
oauth_flows: []
overview: Live Direct Marketing secures its APIs with http bearer, apiKey (header), and cookie session across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Live Direct Marketing
provider_slug: live-direct-marketing-online
scheme_count: 6
schemes:
- api: LDM v3
  bearerFormat: ldm_<64 hex chars> (contract says JWT — the docs and agent card say an opaque key)
  declared_on_operations: 3 (as `bearer`) — the contract marks 1,265 operations with the `jwt` scheme even though the docs say every protected route accepts either credential
  description: Tenant API key for MCP / A2A / SDK / server-to-server clients. Minted in CRM Settings → API Keys with chosen scopes, or auto-issued by POST /api/auth/register (channel mcp|a2a|form) and by the MCP ldm_register tool. "One format, no separate live/test prefix."
  name: tenant-api-key
  scheme: bearer
  scopes: scopes/live-direct-marketing-online-scopes.yml (79 in the card; x-required-scope on 406 operations)
  sources:
  - openapi/live-direct-marketing-online-ldm-v3-openapi.json
  - https://developers.live-direct-marketing.online/authentication
  type: http
- api: LDM v3
  bearerFormat: JWT
  declared_on_operations: 1265
  description: 15-minute access token from POST /api/auth/login (AuthController_login), refreshed with POST /api/auth/refresh; carried by the web UI as an HttpOnly cookie. 401 = wrong credentials; 403 = correct credentials but account not ACTIVE (unconfirmed email / awaiting approval / blocked).
  name: jwt
  scheme: bearer
  sources:
  - openapi/live-direct-marketing-online-ldm-v3-openapi.json
  - https://developers.live-direct-marketing.online/authentication
  type: http
- api: LDM v3
  declared_on_operations: 14
  description: Dedicated RPA service key for the RPA service protocol (14 operations under /api/rpa/v1); "No tenant API-key or query-key authentication."
  name: rpa-service
  scheme: bearer
  sources:
  - openapi/live-direct-marketing-online-ldm-v3-openapi.json
  type: http
- api: Inbox Check
  bearerFormat: icp_live_*
  declared_on_operations: 38
  description: Bearer API key issued at /account (up to 3 active per user, shown once). Carries tier (basic/pro/enterprise), scopes (monitoring:read | monitoring:write | reports:pdf), an optional provider allowlist, a screenshots feature flag and daily/monthly quotas readable at GET /api/v1/me.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/live-direct-marketing-online-inbox-check-openapi.json
  - https://check.live-direct-marketing.online/docs
  type: http
- api: Inbox Check
  declared_on_operations: 64
  description: Operator key for /api/admin/* routes (64 operations). Not available to customers.
  in: header
  name: adminKey
  name_header: X-Admin-Key
  sources:
  - openapi/live-direct-marketing-online-inbox-check-openapi.json
  type: apiKey
- api: Inbox Check
  declared_on_operations: 21
  description: Account-portal session set by POST /api/auth/login; referenced by 21 /api/account/* operations but NEVER DECLARED in components.securitySchemes — a contract defect. Recorded from the security requirements, not from a scheme object.
  in: cookie
  name: cookie
  sources:
  - openapi/live-direct-marketing-online-inbox-check-openapi.json
  type: apiKey
slug: live-direct-marketing-online-authentication
source_filename: live-direct-marketing-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://developers.live-direct-marketing.online/authentication\ndocs:\n  - https://developers.live-direct-marketing.online/authentication\n  - https://developers.live-direct-marketing.online/api-registration\n  - https://developers.live-direct-marketing.online/limits\n  - https://check.live-direct-marketing.online/docs\nspec:\n  - openapi/live-direct-marketing-online-ldm-v3-openapi.json\n  - openapi/live-direct-marketing-online-inbox-check-openapi.json\nsummary:\n  types: [http bearer, apiKey (header), cookie session]\n  api_key_in: [header]\n  oauth2_flows: []\n  transport: 'Authorization header, Bearer scheme, HTTPS only (HSTS on every host)'\n  note: >-\n    Two contracts, five declared security schemes, no OAuth 2.0 authorization server. LDM: one\n    HybridAuthGuard resolves either an HttpOnly JWT cookie session (web UI) or a Bearer ldm_* tenant\n    API key (agents, MCP, A2A, server-to-server) to the same handler, with\
  \ per-method scope checks\n    on Bearer keys. Inbox Check: Bearer icp_live_* keys with tier, scopes, provider allowlist and\n    quotas, plus an X-Admin-Key header for operator routes and a session cookie for the account\n    portal. The derive pass produced the scheme skeleton; this file upgrades it from the docs.\nschemes:\n  - name: tenant-api-key\n    api: LDM v3\n    type: http\n    scheme: bearer\n    bearerFormat: 'ldm_<64 hex chars> (contract says JWT — the docs and agent card say an opaque key)'\n    description: >-\n      Tenant API key for MCP / A2A / SDK / server-to-server clients. Minted in CRM Settings → API\n      Keys with chosen scopes, or auto-issued by POST /api/auth/register (channel mcp|a2a|form) and by\n      the MCP ldm_register tool. \"One format, no separate live/test prefix.\"\n    scopes: scopes/live-direct-marketing-online-scopes.yml (79 in the card; x-required-scope on 406 operations)\n    sources: [openapi/live-direct-marketing-online-ldm-v3-openapi.json,\
  \ https://developers.live-direct-marketing.online/authentication]\n    declared_on_operations: 3 (as `bearer`) — the contract marks 1,265 operations with the `jwt` scheme even though the docs say every protected route accepts either credential\n  - name: jwt\n    api: LDM v3\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      15-minute access token from POST /api/auth/login (AuthController_login), refreshed with\n      POST /api/auth/refresh; carried by the web UI as an HttpOnly cookie. 401 = wrong credentials;\n      403 = correct credentials but account not ACTIVE (unconfirmed email / awaiting approval / blocked).\n    sources: [openapi/live-direct-marketing-online-ldm-v3-openapi.json, https://developers.live-direct-marketing.online/authentication]\n    declared_on_operations: 1265\n  - name: rpa-service\n    api: LDM v3\n    type: http\n    scheme: bearer\n    description: Dedicated RPA service key for the RPA service protocol (14 operations under\
  \ /api/rpa/v1); \"No tenant API-key or query-key authentication.\"\n    sources: [openapi/live-direct-marketing-online-ldm-v3-openapi.json]\n    declared_on_operations: 14\n  - name: apiKey\n    api: Inbox Check\n    type: http\n    scheme: bearer\n    bearerFormat: 'icp_live_*'\n    description: >-\n      Bearer API key issued at /account (up to 3 active per user, shown once). Carries tier\n      (basic/pro/enterprise), scopes (monitoring:read | monitoring:write | reports:pdf), an optional\n      provider allowlist, a screenshots feature flag and daily/monthly quotas readable at GET /api/v1/me.\n    sources: [openapi/live-direct-marketing-online-inbox-check-openapi.json, https://check.live-direct-marketing.online/docs]\n    declared_on_operations: 38\n  - name: adminKey\n    api: Inbox Check\n    type: apiKey\n    in: header\n    name_header: X-Admin-Key\n    description: Operator key for /api/admin/* routes (64 operations). Not available to customers.\n    sources: [openapi/live-direct-marketing-online-inbox-check-openapi.json]\n\
  \    declared_on_operations: 64\n  - name: cookie\n    api: Inbox Check\n    type: apiKey\n    in: cookie\n    description: >-\n      Account-portal session set by POST /api/auth/login; referenced by 21 /api/account/* operations\n      but NEVER DECLARED in components.securitySchemes — a contract defect. Recorded from the\n      security requirements, not from a scheme object.\n    sources: [openapi/live-direct-marketing-online-inbox-check-openapi.json]\n    declared_on_operations: 21\ncredentials:\n  - id: ldm-tenant-key\n    header: 'Authorization: Bearer ldm_...'\n    prefix: ldm_\n    use: Every /api/* route for agents, MCP, A2A and integrations; scope-checked per method\n    issued_by: CRM Settings → API Keys, POST /api/auth/register (agent channels), MCP ldm_register\n    initial_scopes: 'SAFE_AGENT_SCOPES — read-all + safe drafts; no email:send / mailing:write until the owner expands the key after activation'\n  - id: ldm-session\n    header: HttpOnly cookie (JWT, 15 min) after\
  \ https://app.live-direct-marketing.online/login\n    prefix: null\n    use: Web UI; roles OWNER / MANAGER / SUPER grant scopes\n  - id: inbox-check-key\n    header: 'Authorization: Bearer icp_live_...'\n    prefix: icp_live_\n    use: /api/v1/* and /mcp on check.live-direct-marketing.online\n    issued_by: https://check.live-direct-marketing.online/account\n  - id: inbox-check-admin\n    header: 'X-Admin-Key: ...'\n    use: operator only\nanonymous_surfaces:\n  - GET /api/v1/health, GET /api/public/pricing, GET /api/legal/documents[/{key}], GET /api/legal/terms, GET /api/v1/agent-guide, the .well-known cards (LDM)\n  - MCP initialize + tools/list at https://api.live-direct-marketing.online/mcp (bootstrap tools only)\n  - the free Inbox Placement Test web flow (no key; 3 tests per email per day)\nanti_enumeration: 'Any auth failure returns the same generic 401 {\"statusCode\":401,\"message\":\"Invalid credentials\"} — by design.'\noauth:\n  authorization_server: false\n  protected_resource_metadata:\
  \ 'served at /api/v1/.well-known/oauth-protected-resource with authorization_servers: [] (see well-known/)'\n  note: >-\n    The LDM \"OAuth\" tag is the platform acting as an OAuth client toward Gmail / Microsoft for the\n    user's sending mailboxes; Inbox Check's /api/oauth/authorize + /api/oauth/token exist in the\n    contract but are undocumented and unadvertised.\ncontract_gaps:\n  - Both contracts declare bearerFormat JWT for keys the docs describe as opaque prefixed strings.\n  - Inbox Check references an undeclared `cookie` scheme on 21 operations.\n  - LDM declares `jwt` on 1,265 operations and `bearer` (undeclared name) on 3, while the docs state every protected route accepts either the cookie or the tenant key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-direct-marketing-online/refs/heads/main/authentication/live-direct-marketing-online-authentication.yml
summary_line: http bearer/apiKey (header)/cookie session · 6 schemes
tags:
- Company
- Email
- Email Deliverability
- Sales & marketing automation
- CRM
- Lead Management
- Cold Outreach
- Agent-Native
- MCP
- A2A
- Webhook
- B2B
---
