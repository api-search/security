---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agent-ready-dev-openapi.yml
  format: yaml
  label: Agent Ready API
  slug: agent-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agent-ready-dev/refs/heads/main/openapi/agent-ready-dev-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agent Ready Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Ready secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agent Ready
provider_slug: agent-ready-dev
scheme_count: 1
schemes:
- applies_to:
  - startScan
  - listScans
  - getScan
  bearerFormat: ar_live_<prefix>_<secret>
  ci_convention: GitHub Actions secret AGENT_READY_API_KEY; CLI/SDK env var AGENT_READY_API_KEY.
  description: API key issued from /dashboard/api-keys. Pro subscription required.
  header: 'Authorization: Bearer ar_live_<prefix>_<secret>'
  issuance: https://agent-ready.dev/dashboard/api-keys (human-mediated; shown once; Pro plan required)
  key_format: ar_live_<prefix>_<secret> — the prefix is non-secret and identifies the key in the dashboard; only the SHA-256 hash of the secret is stored server-side, so a leaked key must be rotated, not recovered.
  name: ApiKey
  rotation: Two keys can be active simultaneously for zero-downtime rotation; revoke from the dashboard, instant and irreversible.
  scheme: bearer
  shared_surfaces: The same key authenticates REST (/api/v1/scans), the hosted MCP endpoint (/api/v1/mcp) and the A2A endpoint (/api/v1/a2a), and they share one rate-limit budget.
  sources:
  - openapi/agent-ready-dev-openapi.yml
  type: http
slug: agent-ready-dev-authentication
source_filename: agent-ready-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/agent-ready-dev-openapi.yml\ndocs: https://agent-ready.dev/auth\nadditional_docs:\n- https://agent-ready.dev/docs/api#authentication\n- https://agent-ready.dev/.well-known/oauth-protected-resource\n- https://agent-ready.dev/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - http\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  credential_types: [ar_live_ Pro API key]\n  public_operations: [askGet, askPost, scanMcp, x402ScanChallenge, x402Scan]\n  discovery: RFC 9728 protected-resource metadata + RFC 8414 authorization-server metadata + WWW-Authenticate on 401\n  dynamic_client_registration: false\n  delegated_identity: false\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ar_live_<prefix>_<secret>\n  description: API key issued from /dashboard/api-keys. Pro subscription required.\n  sources:\n  - openapi/agent-ready-dev-openapi.yml\n  applies_to: [startScan,\
  \ listScans, getScan]\n  header: 'Authorization: Bearer ar_live_<prefix>_<secret>'\n  key_format: >-\n    ar_live_<prefix>_<secret> — the prefix is non-secret and identifies the key in the dashboard; only the\n    SHA-256 hash of the secret is stored server-side, so a leaked key must be rotated, not recovered.\n  issuance: https://agent-ready.dev/dashboard/api-keys (human-mediated; shown once; Pro plan required)\n  rotation: Two keys can be active simultaneously for zero-downtime rotation; revoke from the dashboard, instant and irreversible.\n  shared_surfaces: The same key authenticates REST (/api/v1/scans), the hosted MCP endpoint (/api/v1/mcp) and the A2A endpoint (/api/v1/a2a), and they share one rate-limit budget.\n  ci_convention: GitHub Actions secret AGENT_READY_API_KEY; CLI/SDK env var AGENT_READY_API_KEY.\nagent_auth:\n  model: machine-to-machine Bearer key (client-credentials-shaped, but issued out of band from a dashboard rather than at a token endpoint)\n  protected_resource_metadata:\n\
  \    url: https://agent-ready.dev/.well-known/oauth-protected-resource\n    file: well-known/agent-ready-dev-oauth-protected-resource.json\n    resource: https://agent-ready.dev/api/v1/mcp\n    authorization_servers: [https://agent-ready.dev]\n    scopes_supported: [scan:read, scan:write, ask:read, mcp]\n  authorization_server_metadata:\n    url: https://agent-ready.dev/.well-known/oauth-authorization-server\n    file: well-known/agent-ready-dev-oauth-authorization-server.json\n    issuer: https://agent-ready.dev\n    grant_types_supported: [urn:ietf:params:oauth:grant-type:api-key]\n    registration_endpoint: https://agent-ready.dev/dashboard/api-keys (human dashboard — not RFC 7591)\n    agent_auth_block: 'register_uri, identity_types_supported [anonymous, identity_assertion], skill https://agent-ready.dev/auth.md'\n  www_authenticate: 'Bearer realm=\"agent-ready\", error=\"invalid_token\", resource_metadata=\"https://agent-ready.dev/.well-known/oauth-protected-resource\"'\n  observed:\
  \ 'GET https://agent-ready.dev/api -> 401 with the WWW-Authenticate challenge above (2026-09-19).'\n  not_supported:\n  - OAuth 2.1 authorization-code flow\n  - RFC 7591 dynamic client registration\n  - RFC 7521 identity_assertion / id-jag token exchange\n  - RFC 7009 revocation endpoint (dashboard revocation only)\n  - OpenID Connect discovery\n  bot_identity:\n    web_bot_auth: true\n    directory: https://agent-ready.dev/.well-known/http-message-signatures-directory\n    note: The provider publishes its own RFC 9421 Ed25519 key directory for the agent-ready-scanner bot; it identifies the bot, the Bearer key authorises the call.\nalternatives_without_a_key:\n  anonymous_free_tier: POST https://agent-ready.dev/api/scan — 3 scans / 30 days per IP at 25-page depth; also what the stdio MCP package and CLI use keyless.\n  mcp_apps_endpoint: https://agent-ready.dev/api/apps/mcp — tools/call with no credential; rate-limited per opaque ChatGPT user id.\n  x402_mpp: 'Pay per scan with an X-PAYMENT\
  \ header or MPP Authorization: Payment on /api/x402/scan — $0.02 / $0.25 USDC on Base, no account.'\n  public_endpoints: [GET/POST /api/v1/ask, POST /api/v1/scan/mcp]\nerrors:\n  401: {code: invalid_token, meaning: Missing, malformed, expired or revoked Bearer token}\n  403: {code: insufficient_scope, meaning: Token valid but the plan tier lacks access (e.g. Free-tier key calling /api/v1/scans); OpenAPI Error example code subscription_required}\n  429: {meaning: 'Over 10/min or 200/day; Retry-After present'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent-ready-dev/refs/heads/main/authentication/agent-ready-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- Agent Readiness
- Website Scanning
- Developer Tools
- MCP
- A2A
- llms-txt
- x402
- NLWeb
- Accessibility
- Agent-Native
- Australia
---
