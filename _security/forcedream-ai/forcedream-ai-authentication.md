---
anonymous_access: true
api_key_in: []
api_specs:
- filename: forcedream-ai-openapi.yml
  format: yaml
  label: ForceDream API
  slug: forcedream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/openapi/forcedream-ai-openapi.yml
auth_types:
- http
- oauth2
description: ForceDream authenticates three ways. REST calls carry a bearer key — either an fd_live_ billing key that spends balance or an sk_fd_ account key for management, both issued together by an anonymous POST /api/signup and shown once. MCP clients use OAuth 2.1 authorization code + PKCE against https://api.forcedream.ai with RFC 7591 dynamic client registration (no pre-shared credential, no human step) and scopes mcp:invoke / mcp:tools; the A2A card names the same flow with scope agent.execute. Discovery, pricing, reliability and proof verification require no credential at all. Human sign-in to the console is GitHub or Google OAuth ("No password storage"). Keys are stored as SHA-256 hashes, revocable immediately.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Forcedream Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ForceDream secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ForceDream
provider_slug: forcedream-ai
scheme_count: 3
schemes:
- description: An `fd_live_` billing key (from signup) or `sk_fd_` account key.
  header: 'Authorization: Bearer <key>'
  issuance: 'POST /api/signup {"email": "..."} -> {live_key, api_key, user_id}; no card, email not verified before issue; rate-limited 5 per IP per hour'
  key_types:
  - env: FD_API_KEY (MCP server), FD_LIVE_KEY (CLI)
    prefix: fd_live_
    role: billing / metered — required for any route or MCP tool that spends balance (invoke, execute_plan, paid search sources)
  - env: FORCEDREAM_API_KEY (SDKs)
    format: sk_fd_{40_hex_characters}
    prefix: sk_fd_
    role: account management — "Distinct from live_key and not interchangeable with it" (agent card)
  name: bearerAuth
  revocation: POST /v1/account/keys/revoke (immediate); multiple keys per account; recovery via POST /api/recover-key
  scheme: bearer
  sources:
  - openapi/forcedream-ai-openapi.yml
  - https://www.forcedream.com/developers/security
  storage: '"API keys are hashed with SHA-256 before storage. The raw key is never stored — only the hash. Key rotation is instant." Shown exactly once at signup.'
  type: http
- description: OAuth 2.1 authorization code with PKCE for MCP clients (and the A2A card); tokens are presented as bearer tokens to https://api.forcedream.ai/v1/mcp.
  detail: scopes/forcedream-ai-scopes.yml
  dynamic_client_registration: RFC 7591 — "Registration requires no pre-shared credential and no human step. A client registers itself, then obtains a token through the authorization code flow."
  flows:
    authorizationCode:
      authorizationUrl: https://api.forcedream.ai/v1/oauth/authorize
      refreshUrl: https://api.forcedream.ai/v1/oauth/token
      scopes:
        agent.execute: Discover, price and execute ForceDream agents, and retrieve the signed record of what ran (A2A card)
        mcp:invoke: Invoke tools that spend balance (AS metadata scopes_supported)
        mcp:tools: Access the tool surface (AS metadata scopes_supported)
      tokenUrl: https://api.forcedream.ai/v1/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.forcedream.ai
  metadata: well-known/forcedream-ai-oauth-authorization-server.json
  name: oauth2
  pkce: S256
  protected_resource_metadata: well-known/forcedream-ai-oauth-protected-resource.json
  registration_endpoint: https://api.forcedream.ai/v1/oauth/register
  sources:
  - well-known/forcedream-ai-oauth-authorization-server.json
  - a2a/forcedream-ai-agent-card.json
  - https://github.com/forcedreamai/forcedream-mcp/blob/main/README.md
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
- applies_to:
  - GET /v1/agents/list, GET /v1/agents/reliability, POST /v1/procure, GET /v1/workforce/proof/{task_id}/public, GET /v1/workforce/proof/public-key, GET /v1/health, GET /v1/status, GET /v1/capabilities, GET /v1/factory/dashboard
  - MCP tools forcedream_search_agents, forcedream_search_costs, forcedream_search_reliability, forcedream_search_providers, forcedream_plan_work, forcedream_verify_proof, forcedream_get_execution; MCP initialize / tools/list / prompts/list / resources/list
  - A2A card and per-agent cards; an anonymous message/send returns an agent greeting
  description: No credential required.
  name: anonymous
  type: none
slug: forcedream-ai-authentication
source_filename: forcedream-ai-authentication.yml
source_heading: Authentication Profile
source_url: openapi/forcedream-ai-openapi.yml (securitySchemes.bearerAuth)
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://www.forcedream.com/developers/security\nsources:\n  - openapi/forcedream-ai-openapi.yml (securitySchemes.bearerAuth)\n  - https://www.forcedream.com/developers/security\n  - https://www.forcedream.com/developers/quickstart\n  - well-known/forcedream-ai-oauth-authorization-server.json (RFC 8414)\n  - well-known/forcedream-ai-oauth-protected-resource.json (RFC 9728)\n  - a2a/forcedream-ai-agent-card.json (securitySchemes, self-service-credentials extension)\n  - https://github.com/forcedreamai/forcedream-mcp/blob/main/README.md\n  - https://github.com/forcedreamai/forcedream-docs/blob/main/docs/security/README.md\n  - https://www.forcedream.com/trust/controls\ndocs: https://www.forcedream.com/developers/security\ndescription: >-\n  ForceDream authenticates three ways. REST calls carry a bearer key — either an fd_live_ billing key that\n  spends balance or an sk_fd_ account key for management, both issued together by an\
  \ anonymous POST /api/signup\n  and shown once. MCP clients use OAuth 2.1 authorization code + PKCE against https://api.forcedream.ai with\n  RFC 7591 dynamic client registration (no pre-shared credential, no human step) and scopes mcp:invoke /\n  mcp:tools; the A2A card names the same flow with scope agent.execute. Discovery, pricing, reliability and\n  proof verification require no credential at all. Human sign-in to the console is GitHub or Google OAuth\n  (\"No password storage\"). Keys are stored as SHA-256 hashes, revocable immediately.\nsummary:\n  types: [http, oauth2]\n  anonymous_surface: true\n  self_service_issuance: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An `fd_live_` billing key (from signup) or `sk_fd_` account key.\n  header: 'Authorization: Bearer <key>'\n  key_types:\n    - prefix: fd_live_\n      role: billing / metered — required for any route or MCP tool that spends balance (invoke, execute_plan, paid search sources)\n  \
  \    env: FD_API_KEY (MCP server), FD_LIVE_KEY (CLI)\n    - prefix: sk_fd_\n      format: sk_fd_{40_hex_characters}\n      role: account management — \"Distinct from live_key and not interchangeable with it\" (agent card)\n      env: FORCEDREAM_API_KEY (SDKs)\n  issuance: 'POST /api/signup {\"email\": \"...\"} -> {live_key, api_key, user_id}; no card, email not verified before issue; rate-limited 5 per IP per hour'\n  storage: '\"API keys are hashed with SHA-256 before storage. The raw key is never stored — only the hash. Key rotation is instant.\" Shown exactly once at signup.'\n  revocation: POST /v1/account/keys/revoke (immediate); multiple keys per account; recovery via POST /api/recover-key\n  sources:\n  - openapi/forcedream-ai-openapi.yml\n  - https://www.forcedream.com/developers/security\n- name: oauth2\n  type: oauth2\n  description: OAuth 2.1 authorization code with PKCE for MCP clients (and the A2A card); tokens are presented as bearer tokens to https://api.forcedream.ai/v1/mcp.\n\
  \  flows:\n    authorizationCode:\n      authorizationUrl: https://api.forcedream.ai/v1/oauth/authorize\n      tokenUrl: https://api.forcedream.ai/v1/oauth/token\n      refreshUrl: https://api.forcedream.ai/v1/oauth/token\n      scopes:\n        'mcp:invoke': Invoke tools that spend balance (AS metadata scopes_supported)\n        'mcp:tools': Access the tool surface (AS metadata scopes_supported)\n        'agent.execute': Discover, price and execute ForceDream agents, and retrieve the signed record of what ran (A2A card)\n  issuer: https://api.forcedream.ai\n  metadata: well-known/forcedream-ai-oauth-authorization-server.json\n  protected_resource_metadata: well-known/forcedream-ai-oauth-protected-resource.json\n  registration_endpoint: https://api.forcedream.ai/v1/oauth/register\n  dynamic_client_registration: RFC 7591 — \"Registration requires no pre-shared credential and no human step. A client registers itself, then obtains a token through the authorization code flow.\"\n  pkce: S256\n\
  \  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none, client_secret_post]\n  detail: scopes/forcedream-ai-scopes.yml\n  sources:\n  - well-known/forcedream-ai-oauth-authorization-server.json\n  - a2a/forcedream-ai-agent-card.json\n  - https://github.com/forcedreamai/forcedream-mcp/blob/main/README.md\n- name: anonymous\n  type: none\n  description: No credential required.\n  applies_to:\n    - GET /v1/agents/list, GET /v1/agents/reliability, POST /v1/procure, GET /v1/workforce/proof/{task_id}/public, GET /v1/workforce/proof/public-key, GET /v1/health, GET /v1/status, GET /v1/capabilities, GET /v1/factory/dashboard\n    - MCP tools forcedream_search_agents, forcedream_search_costs, forcedream_search_reliability, forcedream_search_providers, forcedream_plan_work, forcedream_verify_proof, forcedream_get_execution; MCP initialize / tools/list / prompts/list / resources/list\n    - A2A card and per-agent cards; an anonymous message/send returns an agent\
  \ greeting\nconsole_login:\n  methods: [GitHub OAuth, Google OAuth, email]\n  note: '\"OAuth: GitHub and Google. No password storage.\" (trust/controls)'\nmachine_credential_errors:\n  rest: '401 {\"error\":\"auth_required\"} / {\"error\":\"Invalid API key\"}'\n  mcp: 'JSON-RPC -32001 authentication_required with data.acquisition (signup endpoint, credential field, credit grant) — see errors/forcedream-ai-problem-types.yml'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/authentication/forcedream-ai-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- AI Agents
- Agent Marketplace
- MCP
- A2A
- Cryptographic Proofs
- AI Inference Routing
- Agent Payments
- Agentic Commerce
- agent-native
- United Kingdom
---
