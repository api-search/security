---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cloutjam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CloutJam secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CloutJam
provider_slug: cloutjam
scheme_count: 2
schemes:
- audience: power users, scripted/CLI workflows, agent runtimes
  bearer_prefix: cd_pat_
  env_var: CLOUTDESK_AGENT_PAT
  example: 'Authorization: Bearer cd_pat_…'
  header: Authorization
  in: header
  minted_from: https://dashboard.cloutdesk.com
  name: personalAccessToken
  scheme: bearer
  scope_note: The repo states "Required scopes on the integrator's Cloutdesk PAT", so PATs carry the same scope names as OAuth grants.
  scoped: true
  sources:
  - https://www.cloutdesk.com/agent-platform
  - https://github.com/cloutdesk/agents/blob/main/README.md
  type: http
- audience: organization-wide installs; Claude Managed Agents one-click install
  authorizationUrl: null
  cli_login: npx @cloutdesk/mcp oauth login
  endpoints_published: false
  flow: authorizationCode
  name: oauth2
  pkce: true
  scopes_documented:
  - collaborations:read
  - creators:read
  - events:emit
  - transactions:read
  scopes_marketing_example:
  - campaigns
  - collaborations
  - agreements:write
  sources:
  - https://www.cloutdesk.com/agent-platform
  - https://github.com/cloutdesk/agents
  tokenUrl: null
  type: oauth2
  version: OAuth 2.1
slug: cloutjam-authentication
source_filename: cloutjam-authentication.yml
source_heading: Authentication Profile
source_url: https://www.cloutdesk.com/agent-platform
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.cloutdesk.com/agent-platform\nsources:\n- https://www.cloutdesk.com/agent-platform\n- https://github.com/cloutdesk/agents/blob/main/README.md\nstatus: beta\nnotes: >-\n  UPGRADE over the 2026-07-18 round. No OpenAPI securitySchemes exist to derive from —\n  Cloutdesk publishes no spec — so this profile is searched from the vendor's Agent\n  Platform page and, new this round, from its own public agents repo, which names the\n  environment variables an integrator sets (`CLOUTDESK_API_URL`, `CLOUTDESK_AGENT_PAT`)\n  and states that the PAT is minted from the Cloutdesk dashboard. The OAuth grant is now\n  specified more precisely than before: OAuth 2.1 + PKCE for the Claude Managed Agents\n  one-click install. No authorization or token endpoint URL is published anywhere, and\n  api.cloutdesk.com does not resolve, so no endpoint could be probed or recorded.\nsummary:\n  types: [http, oauth2]\n  http_bearer: true\n  api_key_in:\
  \ [header]\n  oauth2_flows: [authorizationCode]\n  oauth2_pkce: true\n  scope_gated: true\n  scope_count: 4\n  mtls: false\n  openid_connect: false\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  bearer_prefix: cd_pat_\n  example: 'Authorization: Bearer cd_pat_…'\n  audience: power users, scripted/CLI workflows, agent runtimes\n  minted_from: https://dashboard.cloutdesk.com\n  env_var: CLOUTDESK_AGENT_PAT\n  scoped: true\n  scope_note: The repo states \"Required scopes on the integrator's Cloutdesk PAT\", so PATs carry the\n    same scope names as OAuth grants.\n  sources:\n  - https://www.cloutdesk.com/agent-platform\n  - https://github.com/cloutdesk/agents/blob/main/README.md\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  version: OAuth 2.1\n  audience: organization-wide installs; Claude Managed Agents one-click install\n  authorizationUrl: null\n  tokenUrl: null\n  endpoints_published: false\n\
  \  scopes_documented: [collaborations:read, creators:read, events:emit, transactions:read]\n  scopes_marketing_example: [campaigns, collaborations, 'agreements:write']\n  cli_login: npx @cloutdesk/mcp oauth login\n  sources:\n  - https://www.cloutdesk.com/agent-platform\n  - https://github.com/cloutdesk/agents\nper_surface:\n- surface: MCP server\n  auth: OAuth (login via `npx @cloutdesk/mcp oauth login`) or PAT via CLOUTDESK_AGENT_PAT\n- surface: REST API (v1)\n  auth: Bearer PAT (cd_pat_) or OAuth for org-wide installs\n- surface: CLI (cloutdesk)\n  auth: PAT\n- surface: Microsoft 365 Copilot Studio / Workforce Agents\n  auth: 'described as \"Entra ID-friendly authentication\"; no detail published'\nauthorization_model:\n  row_level_security: true\n  rls_detail: 'Agents operate under \"the same row-level permissions as a human teammate\";\n    the platform is described as RLS-enforced.'\n  granular_consent: true\n  sensitive_actions_separately_consented: [e-signature, email send, creator\
  \ ingest]\n  audited: true\n  source: https://www.cloutdesk.com/agent-platform\ndiscovery:\n  well_known_oauth_authorization_server: 404\n  well_known_openid_configuration: 404\n  probed: '2026-08-13'\n  note: Neither RFC 8414 nor OIDC discovery is served on www.cloutdesk.com; see\n    well-known/cloutjam-well-known.yml.\ngaps:\n- No authorization/token endpoint URLs published.\n- No token lifetime, refresh, or rotation policy published.\n- No dedicated authentication docs page; everything above comes from a marketing page and a\n  skills repo README.\ncross_links:\n  scopes: scopes/cloutjam-scopes.yml\n  conventions: conventions/cloutjam-conventions.yml\n  mcp: mcp/cloutjam-mcp.yml\n  well_known: well-known/cloutjam-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloutjam/refs/heads/main/authentication/cloutjam-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Influencer Marketing
- Creator Management
- Creator Economy
- Marketing
- Agentic AI
- Agents
- MCP
- Agent Skills
- Talent Management
- Influencer Marketing Platform
---
