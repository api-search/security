---
api_key_in: []
auth_types: []
description: 'The PulseMCP Registry API is protected by a single API-key scheme carried in a custom request header, plus a second custom header that selects the tenant. There is no OAuth, no OIDC, no mTLS, and no self-service key issuance: keys are granted only by emailing hello@pulsemcp.com, which makes this a sales-gated API with a fully public reference.'
kind: authentication
layout: security
method: searched
name: Pulsemcp Authentication
name_suffix: Authentication
oauth_flows: []
overview: PulseMCP declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PulseMCP
provider_slug: pulsemcp
scheme_count: 2
schemes:
- applies_to: every path, including the utility endpoints /v0.1/health, /v0.1/ping and /v0.1/version
  description: '"Your PulseMCP API key". Sent on every request. A missing or invalid key returns HTTP 401 with body {"error":"Invalid or missing API key","code":"unauthorized","details":{"header":"X-API-Key"}} — observed live on 2026-08-13.'
  id: apiKeyHeader
  in: header
  key_format: not published
  name: X-API-Key
  required: true
  rotation_policy: not published
  type: apiKey
- applies_to: All data endpoints (/v0.1/servers and below). Documented as optional only for the utility endpoints (health, ping, version).
  description: '"Your tenant identifier". Selects which curated sub-registry view the key reads. The MCP server validates it against /^[a-zA-Z0-9_-]*$/ with a 256 character maximum, and can switch it at runtime via its switch_tenant_id admin tool.'
  id: tenantHeader
  in: header
  name: X-Tenant-ID
  required: conditional
  type: apiKey
slug: pulsemcp-authentication
source_filename: pulsemcp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://www.pulsemcp.com/api/docs/v0.1 (authentication section), corroborated by\n  live 401 responses from https://api.pulsemcp.com/v0.1/servers and\n  /v0.1/health, and by the first-party client at\n  https://github.com/pulsemcp/mcp-servers/blob/main/productionized/pulse-subregistry/shared/src/client.ts\ndescription: >-\n  The PulseMCP Registry API is protected by a single API-key scheme carried in a\n  custom request header, plus a second custom header that selects the tenant.\n  There is no OAuth, no OIDC, no mTLS, and no self-service key issuance: keys are\n  granted only by emailing hello@pulsemcp.com, which makes this a sales-gated API\n  with a fully public reference.\nbase_url: https://api.pulsemcp.com\ndocs: https://www.pulsemcp.com/api/docs/v0.1\nderived_from_openapi: false\nopenapi_present: false\n\nschemes:\n  - id: apiKeyHeader\n    type: apiKey\n    in: header\n    name: X-API-Key\n    required: true\n\
  \    applies_to: every path, including the utility endpoints /v0.1/health, /v0.1/ping and /v0.1/version\n    description: >-\n      \"Your PulseMCP API key\". Sent on every request. A missing or invalid key\n      returns HTTP 401 with body\n      {\"error\":\"Invalid or missing API key\",\"code\":\"unauthorized\",\"details\":{\"header\":\"X-API-Key\"}} —\n      observed live on 2026-08-13.\n    key_format: not published\n    rotation_policy: not published\n  - id: tenantHeader\n    type: apiKey\n    in: header\n    name: X-Tenant-ID\n    required: conditional\n    applies_to: >-\n      All data endpoints (/v0.1/servers and below). Documented as optional only for\n      the utility endpoints (health, ping, version).\n    description: >-\n      \"Your tenant identifier\". Selects which curated sub-registry view the key\n      reads. The MCP server validates it against /^[a-zA-Z0-9_-]*$/ with a 256\n      character maximum, and can switch it at runtime via its switch_tenant_id\n      admin\
  \ tool.\n\noauth2: false\nopenid_connect: false\nmutual_tls: false\nbasic_auth: false\nbearer_token: false\n\nkey_acquisition:\n  self_service: false\n  signup_url: null\n  process: >-\n    Email hello@pulsemcp.com. The /api page states PulseMCP is \"working directly\n    with partners to provide an enriched, curated, quality-controlled MCP server\n    registry offering customized to the needs of the partner business\" — there is\n    no signup form, no developer dashboard, and no free tier documented.\n  premium_activation: >-\n    Several response fields (remotes[].isSelfHosted, remotes[].authOptions,\n    remotes[].tools, packages[].authOptions, packages[].tools) are marked Premium\n    and are activated per tenant by contacting hello@pulsemcp.com.\n\nfailure_modes:\n  - status: 401\n    code: unauthorized\n    meaning: Missing or invalid API key.\n  - status: 403\n    code: forbidden\n    meaning: Valid API key but access denied (e.g. tenant not entitled).\n\nenvironment_variables_note:\
  \ >-\n  The first-party @pulsemcp/pulse-subregistry MCP server maps these headers to\n  environment variables.\nenvironment_variables:\n  - name: PULSEMCP_SUBREGISTRY_API_KEY\n    maps_to: X-API-Key\n    required: true\n  - name: PULSEMCP_SUBREGISTRY_TENANT_ID\n    maps_to: X-Tenant-ID\n    required: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulsemcp/refs/heads/main/authentication/pulsemcp-authentication.yml
summary_line: 2 schemes
tags:
- MCP
- AI Agents
- Agentic Engineering
- Directory
- Registry
- Community
- Developer Tools
- LLM Tooling
- Newsletter
---
