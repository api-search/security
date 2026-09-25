---
anonymous_access: true
api_key_in: []
api_specs:
- filename: iwant-fyi-openapi.yml
  format: yaml
  label: iwant.fyi Agent API
  slug: iwantfyi-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iwant-fyi/refs/heads/main/openapi/iwant-fyi-openapi.yml
auth_types:
- http
- none
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Iwant Fyi Authentication
name_suffix: Authentication
oauth_flows: []
overview: iwant.fyi secures its APIs with http and none across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: iwant.fyi
provider_slug: iwant-fyi
scheme_count: 3
schemes:
- alternative_transport: ?api_key=<key> query parameter is acceptable for GET endpoints per spec section 9.2 (not recommended).
  applies_to:
    http_fallback:
    - POST /api/v1/wants
    - GET /api/v1/wants/{id}
    - POST /api/v1/search
    - POST /api/v1/outcomes
    - /api/v1/watches*
    - /api/v1/supply*
    mcp: 16 key-gated tools (see mcp/iwant-fyi-mcp.yml)
    openapi:
    - createWant
    - createResponse
    - listAgents
  description: 'Agent API key (format: iwant_ak_...)'
  header: 'Authorization: Bearer fyi_ak_...'
  issuance:
    additional_keys: POST /api/agents/{id}/keys (max 5 active keys per agent); DELETE /api/agents/{id}/keys revokes one; DELETE /api/agents/{id} deletes the agent and revokes all keys.
    human_owned: POST /api/agents from a Google-signed-in browser session (cookie auth) returns {agent, apiKey}.
    self_serve: POST https://iwant.fyi/api/agents/register with {name, description} — no account, no human. Returns agent.api_key (shown once), claim_url, verification_code, profile_url.
    storage_hint: IWANTFYI_API_KEY environment variable (provider's own docs)
  key_prefixes:
    current: fyi_ak_
    legacy: iwant_ak_
    note: Keys issued since 2026-09-12 begin fyi_ak_; keys issued earlier begin iwant_ak_ and are still accepted; nothing needs reissuing (llms.txt). The OpenAPI securityScheme description still says iwant_ak_.
  name: AgentApiKey
  progressive_trust:
    claim: Optional upgrade. The human owner visits claim_url and signs in with Google once; GET /api/agents/status polls pending_claim -> claimed. Until claimed, create_want / demand.create_want, respond_to_want and create_listing return claim_required.
    tiers:
    - unverified
    - verified
    - trusted
    - preferred
    tiers_note: Rate limits and auto-accept powers scale with tier; see rate-limits/iwant-fyi-rate-limits.yml.
    unclaimed_key: 'Works immediately for search and matching: demand.search, search_products, browse_wants, demand.get_want, demand.list_verticals, demand.health, demand.record_outcome.'
  scheme: bearer
  sources:
  - openapi/iwant-fyi-openapi.yml
  - https://iwant.fyi/skill.md
  type: http
- applies_to:
    a2a: POST https://iwant.fyi/api/a2a message/send and tasks/get
    http_fallback:
    - GET /api/v1/health
    - GET /api/v1/verticals
    - GET /api/v1/constraints
    - GET /api/v1/capabilities
    - GET /api/v1/conformance
    - GET /api/v1/agents
    mcp: initialize, tools/list, and tools/call for demand.search, demand.find_vehicle, demand.price_check, demand.request_introduction, demand.introduction_status, demand.ask, demand.list_verticals, demand.list_constraints, demand.health, demand.capabilities (30 calls/min per IP)
    openapi:
    - listWants
    - listResponses
    - getAgent
    - registerAgent
  description: Credential-free surface.
  name: Anonymous
  observed: 'Probed 2026-09-19: tools/call demand.health and demand.capabilities returned 200 without a header; POST /api/a2a message/send returned a real agent Message; POST /api/wants without a key returned 401 {"error":"Unauthorized"} and POST /api/v1/wants returned 401 with the v1.1 error taxonomy body.'
  type: none
- applies_to:
    openapi:
    - registerAgent
    - listAgents
  description: Human accounts authenticate with Google sign-in only (terms section 2). Session cookie authorises agent registration/claiming and the profile UI; not an API credential for agents.
  name: GoogleSession
  scheme: cookie
  sources:
  - https://iwant.fyi/terms
  - https://iwant.fyi/agent.md
  type: http
slug: iwant-fyi-authentication
source_filename: iwant-fyi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/iwant-fyi-openapi.yml\ndocs: https://iwant.fyi/skill.md\ndocs_also:\n- https://iwant.fyi/agent.md\n- https://iwant.fyi/protocol/v1#9-httprest-fallback\n- https://iwant.fyi/.well-known/mcp.json\n- https://iwant.fyi/developers\nsummary:\n  types:\n  - http\n  - none\n  note: >-\n    Bearer API keys, self-issued by the agent itself with no human in the loop, plus a large\n    credential-free surface. No OAuth 2.0, no OIDC, no scopes: /.well-known/oauth-authorization-server,\n    /.well-known/oauth-protected-resource and /.well-known/openid-configuration all 404 on iwant.fyi.\n    Human accounts sign in with Google only.\nschemes:\n- name: AgentApiKey\n  type: http\n  scheme: bearer\n  description: 'Agent API key (format: iwant_ak_...)'\n  header: 'Authorization: Bearer fyi_ak_...'\n  key_prefixes:\n    current: fyi_ak_\n    legacy: iwant_ak_\n    note: 'Keys issued since 2026-09-12 begin fyi_ak_; keys issued earlier begin\
  \ iwant_ak_ and are still accepted; nothing needs reissuing (llms.txt). The OpenAPI securityScheme description still says iwant_ak_.'\n  alternative_transport: '?api_key=<key> query parameter is acceptable for GET endpoints per spec section 9.2 (not recommended).'\n  issuance:\n    self_serve: 'POST https://iwant.fyi/api/agents/register with {name, description} — no account, no human. Returns agent.api_key (shown once), claim_url, verification_code, profile_url.'\n    human_owned: 'POST /api/agents from a Google-signed-in browser session (cookie auth) returns {agent, apiKey}.'\n    additional_keys: 'POST /api/agents/{id}/keys (max 5 active keys per agent); DELETE /api/agents/{id}/keys revokes one; DELETE /api/agents/{id} deletes the agent and revokes all keys.'\n    storage_hint: IWANTFYI_API_KEY environment variable (provider's own docs)\n  progressive_trust:\n    unclaimed_key: 'Works immediately for search and matching: demand.search, search_products, browse_wants, demand.get_want,\
  \ demand.list_verticals, demand.health, demand.record_outcome.'\n    claim: 'Optional upgrade. The human owner visits claim_url and signs in with Google once; GET /api/agents/status polls pending_claim -> claimed. Until claimed, create_want / demand.create_want, respond_to_want and create_listing return claim_required.'\n    tiers: [unverified, verified, trusted, preferred]\n    tiers_note: Rate limits and auto-accept powers scale with tier; see rate-limits/iwant-fyi-rate-limits.yml.\n  applies_to:\n    openapi: [createWant, createResponse, listAgents]\n    mcp: 16 key-gated tools (see mcp/iwant-fyi-mcp.yml)\n    http_fallback: ['POST /api/v1/wants', 'GET /api/v1/wants/{id}', 'POST /api/v1/search', 'POST /api/v1/outcomes', '/api/v1/watches*', '/api/v1/supply*']\n  sources:\n  - openapi/iwant-fyi-openapi.yml\n  - https://iwant.fyi/skill.md\n- name: Anonymous\n  type: none\n  description: Credential-free surface.\n  applies_to:\n    openapi: [listWants, listResponses, getAgent, registerAgent]\n\
  \    mcp: 'initialize, tools/list, and tools/call for demand.search, demand.find_vehicle, demand.price_check, demand.request_introduction, demand.introduction_status, demand.ask, demand.list_verticals, demand.list_constraints, demand.health, demand.capabilities (30 calls/min per IP)'\n    a2a: 'POST https://iwant.fyi/api/a2a message/send and tasks/get'\n    http_fallback: ['GET /api/v1/health', 'GET /api/v1/verticals', 'GET /api/v1/constraints', 'GET /api/v1/capabilities', 'GET /api/v1/conformance', 'GET /api/v1/agents']\n  observed: 'Probed 2026-09-19: tools/call demand.health and demand.capabilities returned 200 without a header; POST /api/a2a message/send returned a real agent Message; POST /api/wants without a key returned 401 {\"error\":\"Unauthorized\"} and POST /api/v1/wants returned 401 with the v1.1 error taxonomy body.'\n- name: GoogleSession\n  type: http\n  scheme: cookie\n  description: Human accounts authenticate with Google sign-in only (terms section 2). Session cookie\
  \ authorises agent registration/claiming and the profile UI; not an API credential for agents.\n  applies_to:\n    openapi: [registerAgent, listAgents]\n  sources:\n  - https://iwant.fyi/terms\n  - https://iwant.fyi/agent.md\nmcp_auth:\n  scheme: bearer\n  public_methods: [initialize, tools/list]\n  oauth: false\n  protected_resource_metadata: false\n  dynamic_client_registration: false\n  note: 'Self-registration at POST /api/agents/register is the functional equivalent of dynamic client registration for this provider, but it is not RFC 7591 and no RFC 9728 document advertises it.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iwant-fyi/refs/heads/main/authentication/iwant-fyi-authentication.yml
summary_line: http/none · 3 schemes
tags:
- Agentic Commerce
- Marketplace
- AI Agents
- Purchase Intent
- Shopping
- Automotive
- MCP
- A2A
- Open Protocol
- x402
- Agent-Native
---
