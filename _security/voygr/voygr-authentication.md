---
api_key_in: []
api_specs:
- filename: voygr-calls-api-openapi.yml
  format: yaml
  label: Voygr Calls API
  slug: voygr-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voygr/refs/heads/main/openapi/voygr-calls-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Voygr Authentication
name_suffix: Authentication
oauth_flows: []
overview: VOYGR declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: VOYGR
provider_slug: voygr
scheme_count: 1
schemes:
- applies_to: every operation except GET /health
  description: Issued per customer. Sent on every request. The Business Validation API at dev.voygr.tech uses the same header.
  id: api-key-header
  in: header
  key_format:
    prefix: pk_live_
    source: Observed in the dev-tools README examples (`voygr login pk_live_abc123`). The Calls API documentation never prints a key format because keys are emailed, never displayed.
  name: X-API-Key
  required: true
  type: apiKey
slug: voygr-authentication
source_filename: voygr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://api.voygr.tech/openapi.json (info.description \"## Authentication\"),\n  https://api.voygr.tech/docs, https://api.voygr.tech/checkout,\n  https://github.com/voygr-tech/callwright-skill (SKILL.md \"## Connection\"),\n  https://github.com/voygr-tech/dev-tools (README \"## Authentication\")\ndocs: https://api.voygr.tech/docs\nsummary: >-\n  Single-factor API key in a custom header. No OAuth, no OIDC, no mTLS, no\n  bearer tokens, no scopes. One key carries the customer's credit quota, rate\n  limits and concurrent-call cap.\nschemes:\n- id: api-key-header\n  type: apiKey\n  in: header\n  name: X-API-Key\n  required: true\n  applies_to: every operation except GET /health\n  description: >-\n    Issued per customer. Sent on every request. The Business Validation API at\n    dev.voygr.tech uses the same header.\n  key_format:\n    prefix: pk_live_\n    source: >-\n      Observed in the dev-tools README examples (`voygr\
  \ login pk_live_abc123`).\n      The Calls API documentation never prints a key format because keys are\n      emailed, never displayed.\nspec_gap:\n  securitySchemes_declared: false\n  security_applied: false\n  detail: >-\n    The published OpenAPI 3.1.0 declares NO components.securitySchemes and no\n    top-level or per-operation `security` block. Authentication is expressed\n    only as an optional `X-API-Key` header PARAMETER on each operation\n    (required: false in the schema) plus prose in info.description. A generated\n    client or an agent reading the contract mechanically will not learn that the\n    API is authenticated, and will not mark the header required. This is the\n    single highest-value contract fix available to VOYGR — see\n    overlays/voygr-calls-api-overlay.yaml for the corrective overlay.\nissuance:\n  self_serve: true\n  flow:\n  - step: Request a key\n    how: >-\n      https://api.voygr.tech/checkout (\"Get free API key\", name + email) or\n      POST /signup\
  \ with {\"name\": \"...\", \"email\": \"...\"}\n    auth_required: false\n  - step: Receive the key\n    how: >-\n      Emailed. The key is never shown in the browser and never returned in an\n      API response.\n  - step: Verify\n    how: 'curl -s -H \"X-API-Key: $KEY\" https://api.voygr.tech/users/me'\n  free_tier: 2,500 credits, 25 calls/day cap\nrotation_recovery:\n  endpoint: https://api.voygr.tech/recover\n  cli: voygr recover <email>\n  behavior: >-\n    A recovery link is emailed. Clicking it ROTATES the key — the existing key\n    stops working immediately and a new one is emailed to the same address.\n    Remaining quota and plan tier carry over.\n  enumeration_resistance: >-\n    The response is uniform whether or not the email is registered, and is\n    rate-limited per email and per source IP (dev-tools README).\n  self_service_rotation_from_api: false\nstorage_guidance_published_by_provider:\n- Store the key in the CALLWRIGHT_API_KEY environment variable; never echo or print\
  \ it.\n- 'CLI/library resolution order: --api-key flag, then VOYGR_API_KEY env var, then ~/.config/voygr/config.json.'\n- 'SKILL.md instructs agents: reference the key as $CALLWRIGHT_API_KEY in shell commands, never inline the value.'\n- 'Recommended file mode for the saved env file: 600.'\nfailure_modes:\n- status: 401\n  error_code: AUTHENTICATION_ERROR\n  meaning: Missing or invalid X-API-Key header.\n- status: 403\n  error_code: AUTHENTICATION_ERROR\n  meaning: Invalid, revoked, or unauthorized API key; key not permitted for this request.\nscopes:\n  supported: false\n  note: >-\n    No OAuth and no permission scopes exist. Entitlement is expressed as a key\n    TIER (free / paid / enterprise, surfaced on GET /v1/usage as `tier`) plus a\n    credit balance and a concurrency cap, not as scopes. scopes/ is\n    deliberately not emitted.\ntransport:\n  https_required: true\n  observed_tls: TLSv1.2 on api.voygr.tech (see security/voygr-domain-security.yml)\n  hsts: not sent by api.voygr.tech\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voygr/refs/heads/main/authentication/voygr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Location Intelligence
- POI Data
- Data Enrichment
- Data Validation
- Geospatial
- Places
- AI Agents
- Agent Skills
- Voice AI
- Telephony
- Outbound Calls
- Business Validation
- Y Combinator
---
