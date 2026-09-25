---
anonymous_access: false
api_key_in: []
api_specs:
- filename: humanmirror-fr-x402-openapi.yml
  format: yaml
  label: HumanMirror X402 API
  slug: x402
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-x402-openapi.yml
- filename: humanmirror-fr-sanitize-shield-openapi.yml
  format: yaml
  label: HumanMirror M2M Core Services
  slug: m2m-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-sanitize-shield-openapi.yml
- filename: humanmirror-fr-oracle-openapi.yml
  format: yaml
  label: HumanMirror Oracle API
  slug: oracle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-oracle-openapi.yml
- filename: humanmirror-fr-forge-openapi.yml
  format: yaml
  label: HumanMirror Forge API
  slug: forge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-forge-openapi.yml
- filename: humanmirror-fr-nexus-openapi.yml
  format: yaml
  label: HumanMirror Nexus API
  slug: nexus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-nexus-openapi.yml
- filename: humanmirror-fr-agentops-openapi.yml
  format: yaml
  label: HumanMirror AgentOps API
  slug: agentops
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-agentops-openapi.yml
- filename: humanmirror-fr-magnet-openapi.yml
  format: yaml
  label: HumanMirror Magnet API
  slug: magnet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-magnet-openapi.yml
- filename: humanmirror-fr-outcome-openapi.yml
  format: yaml
  label: HumanMirror Outcome API
  slug: outcome
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-outcome-openapi.yml
- filename: humanmirror-fr-one-openapi.yml
  format: yaml
  label: HumanMirror One API
  slug: one
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-one-openapi.yml
- filename: humanmirror-fr-flow-openapi.yml
  format: yaml
  label: HumanMirror Flow API
  slug: flow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-flow-openapi.yml
- filename: humanmirror-fr-market-openapi.yml
  format: yaml
  label: HumanMirror Intent Market API
  slug: market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-market-openapi.yml
- filename: humanmirror-fr-agent-os-openapi.yml
  format: yaml
  label: HumanMirror Agent OS API
  slug: agent-os
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-agent-os-openapi.yml
- filename: humanmirror-fr-physical-oracle-openapi.yml
  format: yaml
  label: HumanMirror Physical Oracle API
  slug: physical-oracle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-physical-oracle-openapi.yml
- filename: humanmirror-fr-automata-openapi.yml
  format: yaml
  label: HumanMirror Automata API
  slug: automata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-automata-openapi.yml
auth_types:
- http bearer (per-product prefixed API keys)
- apiKey in header (X-API-Key, HumanMirror Pro)
- x402 payment signature (PAYMENT-SIGNATURE header, not an OpenAPI securityScheme)
- none (discovery, quotes, verification, Magnet, MCP tools/list)
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Humanmirror Fr Authentication
name_suffix: Authentication
oauth_flows: []
overview: HumanMirror secures its APIs with http bearer (per-product prefixed API keys), apiKey in header (X-API-Key, HumanMirror Pro), x402 payment signature (PAYMENT-SIGNATURE header, not an OpenAPI securityScheme), and none (discovery, quotes, verification, Magnet, MCP tools/list) across 11 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HumanMirror
provider_slug: humanmirror-fr
scheme_count: 11
schemes:
- bearerFormat: null
  description: Active HumanMirror Pro API key. Grants Next-Gen Preview access subject to the Pro monthly API quota.
  in: header
  name: HumanMirrorProApiKey
  parameter: X-API-Key
  scheme: null
  source: openapi/humanmirror-fr-x402-openapi.yml
  type: apiKey
- bearerFormat: hmep1
  description: Active HumanMirror Enterprise Fleet pass. Next-Gen Preview is included.
  in: null
  name: EnterpriseBearer
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-x402-openapi.yml
  type: http
- bearerFormat: hm_omni_*
  description: HumanMirror Omni-Sync API key. One credit per Shared Context operation when credits are available.
  in: null
  name: OmniSyncApiKey
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-x402-openapi.yml
  type: http
- bearerFormat: hm_oracle_…
  description: null
  in: null
  name: ApiKeyBearer
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-oracle-openapi.yml
  type: http
- bearerFormat: hm_forge_*
  description: null
  in: null
  name: BearerAuth
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-forge-openapi.yml
  type: http
- bearerFormat: hm_nexus_*
  description: null
  in: null
  name: BearerAuth
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-nexus-openapi.yml
  type: http
- bearerFormat: hm_nexus_*
  description: null
  in: null
  name: NexusBearer
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-agentops-openapi.yml
  type: http
- bearerFormat: hm_nexus_*
  description: null
  in: null
  name: BearerAuth
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-outcome-openapi.yml
  type: http
- bearerFormat: hm_nexus_*
  description: null
  in: null
  name: BearerAuth
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-one-openapi.yml
  type: http
- bearerFormat: hm_nexus_*
  description: null
  in: null
  name: BearerAuth
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-flow-openapi.yml
  type: http
- bearerFormat: null
  description: null
  in: null
  name: bearerAuth
  parameter: null
  scheme: bearer
  source: openapi/humanmirror-fr-physical-oracle-openapi.yml
  type: http
slug: humanmirror-fr-authentication
source_filename: humanmirror-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://humanmirror.fr/connect/, https://humanmirror.fr/docs/vibecode/, https://humanmirror.fr/llms.txt,\n  https://humanmirror.fr/skill.md, https://humanmirror.fr/.well-known/mcp.json, /forge-mcp.json, /nexus.json, the\n  three registry server.json files, and every securityScheme in the 16 contracts under openapi/ (listed verbatim\n  below); live 402 challenge observed 2026-09-19\ndocs:\n- https://humanmirror.fr/connect/\n- https://humanmirror.fr/docs/vibecode/\n- https://humanmirror.fr/llms.txt\nsummary:\n  types:\n  - http bearer (per-product prefixed API keys)\n  - apiKey in header (X-API-Key, HumanMirror Pro)\n  - x402 payment signature (PAYMENT-SIGNATURE header, not an OpenAPI securityScheme)\n  - none (discovery, quotes, verification, Magnet, MCP tools/list)\n  oauth2: false\n  oidc: false\n  mtls: false\n  note: 'No OAuth anywhere: /.well-known/oauth-authorization-server, oauth-protected-resource and openid-configuration\n\
  \    all 404. Identity is a bearer key whose PREFIX names the product that issued it, and on pay-per-call routes\n    the credential is the payment itself.'\ncredential_classes:\n- name: Nexus key\n  header: 'Authorization: Bearer hm_nexus_…'\n  products:\n  - Nexus\n  - Outcome\n  - One\n  - Flow\n  - AgentOps\n  how_to_get: POST https://humanmirror.fr/api/nexus/trial/ (100 free credits, one trial per network origin per 90\n    days; 409 if already issued) or Stripe checkout POST /api/nexus/checkout/ then POST /api/nexus/claim/\n  spec_schemes:\n  - NexusBearer\n  - BearerAuth\n- name: Forge key\n  header: 'Authorization: Bearer hm_forge_…'\n  products:\n  - Forge\n  how_to_get: POST https://humanmirror.fr/api/forge/trial (25 calls) or the 4.99 EUR pack\n  spec_schemes:\n  - BearerAuth (forge)\n- name: Oracle key\n  header: 'Authorization: Bearer hm_oracle_…'\n  products:\n  - Oracle\n  how_to_get: 4.99 EUR pack (100 credits) via Stripe\n  spec_schemes:\n  - ApiKeyBearer\n- name: Omni-Sync\
  \ key\n  header: 'Authorization: Bearer hm_omni_…'\n  products:\n  - Omni-Sync\n  - Shared Context Engine (credits first, x402 fallback)\n  how_to_get: POST /api/omni-sync/checkout/ (1.99 / 9.99 / 49.99 EUR packs)\n  spec_schemes:\n  - OmniSyncApiKey\n- name: Enterprise Guard key\n  header: 'Authorization: Bearer hm_guard_…'\n  products:\n  - Enterprise Guard preflight (/api/v1/enterprise-guard/preflight/)\n  how_to_get: Enterprise Guard subscription (1 500 / 3 000 / 5 000 EUR per month)\n  spec_schemes: []\n  note: documented on /enterprise-guard/ only; no OpenAPI\n- name: HumanMirror Pro key\n  header: 'X-API-Key: <key> (README example prefix hm_live_)'\n  products:\n  - Pro SaaS (/api/v1/saas/*)\n  - Next-Gen preview routes (/v1/agent/intent-proof/, /v1/fleet/consensus-lock/, /v1/m2m/escrow-settle/, /v1/agent/state-and-trust/)\n    subject to the Pro monthly quota\n  how_to_get: HumanMirror Pro subscription, 49 EUR/month (https://humanmirror.fr/dashboard/)\n  spec_schemes:\n  - HumanMirrorProApiKey\n\
  - name: Enterprise Fleet pass\n  header: 'Authorization: Bearer <hmep1 token>'\n  products:\n  - Unlimited Payload Normalizer + Consensus Oracle + Sanitize Shield for 30 days; Next-Gen preview included; referral\n    routes\n  how_to_get: POST https://humanmirror.fr/api/x402/enterprise-pass/ paying 297 USDC via x402\n  spec_schemes:\n  - EnterpriseBearer\n- name: Genesis allocation token\n  header: 'Authorization: Bearer <GENESIS_ALLOCATION_TOKEN>'\n  products:\n  - POST /api/v1/m2m/resource/ (20 context_compress calls / 48h)\n  how_to_get: POST /api/v1/m2m/handshake/ then POST /api/v1/m2m/claim-resource/ (skill.md)\n  spec_schemes: []\n- name: x402 payment signature\n  header: 'PAYMENT-SIGNATURE: <EIP-3009 authorization for the exact USDC amount>'\n  products:\n  - every /api/x402/* route, /api/v1/m2m/*, /api/v1/consensus/verify/, /api/v1/sanitize/shield/, /api/v1/zero/,\n    /api/market/intent|award, /v1/agent/perception-vector/, Agent OS state-and-trust\n  how_to_get: Call without it,\
  \ read the PAYMENT-REQUIRED header on the 402 (x402Version 2, accepts[] amount/payTo/network\n    eip155:8453/asset USDC), sign, retry\n  observed: '2026-09-19: POST /api/x402/secret-scanning/ -> 402 ''PAYMENT-SIGNATURE header is required'''\n  spec_schemes: []\n  note: Declared as a header parameter on 68 operations rather than as a securityScheme.\n- name: Anonymous\n  header: null\n  products:\n  - MCP initialize/tools/list on all seven servers\n  - GET discovery endpoints (/api/v1/sanitize/shield/, /api/v1/m2m/payload-normalizer/, /api/v1/consensus/verify/,\n    /api/v1/sink/, /api/v1/zero/, /api/automata, /api/magnet/*, /api/market/live/)\n  - POST /api/outcome/quote/, /api/outcome/verify/, /api/flow/quote/, /api/solve/, /api/nexus/search, /api/trace/verify\n  how_to_get: nothing\n  spec_schemes: []\nschemes:\n- name: HumanMirrorProApiKey\n  type: apiKey\n  scheme: null\n  in: header\n  parameter: X-API-Key\n  bearerFormat: null\n  description: Active HumanMirror Pro API key. Grants\
  \ Next-Gen Preview access subject to the Pro monthly API quota.\n  source: openapi/humanmirror-fr-x402-openapi.yml\n- name: EnterpriseBearer\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hmep1\n  description: Active HumanMirror Enterprise Fleet pass. Next-Gen Preview is included.\n  source: openapi/humanmirror-fr-x402-openapi.yml\n- name: OmniSyncApiKey\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_omni_*\n  description: HumanMirror Omni-Sync API key. One credit per Shared Context operation when credits are available.\n  source: openapi/humanmirror-fr-x402-openapi.yml\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_oracle_…\n  description: null\n  source: openapi/humanmirror-fr-oracle-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_forge_*\n  description: null\n  source: openapi/humanmirror-fr-forge-openapi.yml\n\
  - name: BearerAuth\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_nexus_*\n  description: null\n  source: openapi/humanmirror-fr-nexus-openapi.yml\n- name: NexusBearer\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_nexus_*\n  description: null\n  source: openapi/humanmirror-fr-agentops-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_nexus_*\n  description: null\n  source: openapi/humanmirror-fr-outcome-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_nexus_*\n  description: null\n  source: openapi/humanmirror-fr-one-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: null\n  parameter: null\n  bearerFormat: hm_nexus_*\n  description: null\n  source: openapi/humanmirror-fr-flow-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: null\n  parameter:\
  \ null\n  bearerFormat: null\n  description: null\n  source: openapi/humanmirror-fr-physical-oracle-openapi.yml\nkey_prefix_map:\n  hm_nexus_: Nexus / Outcome / One / Flow / AgentOps\n  hm_forge_: Forge\n  hm_oracle_: Oracle\n  hm_omni_: Omni-Sync / Shared Context\n  hm_guard_: Enterprise Guard\n  hm_live_: Pro (X-API-Key, README example)\n  hmep1: Enterprise Fleet pass bearerFormat\nprivacy_note: The privacy policy states HumanMirror stores a cryptographic digest of the API key, a request id,\n  route, tool, hashed IP, status, latency and credits — not raw payloads.\nnotes:\n- 'The derive-authentication.py baseline (method: derived) merged nine differently named bearer schemes into one\n  row because they share type/scheme; this searched profile keeps each scheme with its own bearerFormat and source.'\n- Keys are never sent as query parameters; every scheme is a header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/authentication/humanmirror-fr-authentication.yml
summary_line: http bearer (per-product prefixed API keys)/apiKey in header (X-API-Key, HumanMirror Pro)/x402 payment signature (PAYMENT-SIGNATURE header, not an OpenAPI securityScheme)/none (discovery, quotes, verification, Magnet, MCP tools/list) · 11 schemes
tags:
- Company
- AI Agents
- Agent Security
- Prompt Injection Defense
- x402
- Machine Payments
- USDC
- MCP
- A2A
- Data Quality
- Verified Outcomes
- Microtransactions
- France
---
