---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: rettfrabonden-com-openapi.yml
  format: yaml
  label: Rett fra Bonden Local Food API
  slug: rett-fra-bonden-local-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/openapi/rettfrabonden-com-openapi.yml
auth_types:
- apiKey
- none
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rettfrabonden Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rett fra Bonden secures its APIs with apiKey and none across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rett fra Bonden
provider_slug: rettfrabonden-com
scheme_count: 4
schemes:
- description: API key received upon registration. Required for write operations; read/search operations are open.
  in: header
  name: apiKey
  obtain: 'issued in the response to POST /api/marketplace/register (openapi.json: "Registered agent with API key"; protected-resource x-auth-obtain-url)'
  parameter: X-API-Key
  required_for:
  - registerProducer
  - producer-side writes documented as "write operations"
  role: producer key
  scopes:
  - write
  sources:
  - a2a/rettfrabonden-com-agent-card.json
  - well-known/rettfrabonden-com-oauth-protected-resource.json
  - well-known/rettfrabonden-com-mcp-server-card.json
  type: apiKey
- description: Free, voluntary key — same header name as the producer key, different purpose; nothing requires it.
  effect: about 3x higher rate-limit ceiling on the general REST and /a2a surface (300 -> 900 and 200 -> 600 per 15 minutes) and a per-key usage ledger (endpoint/tool name and date only); does NOT raise the static 150-per-15-minute quota on /api/marketplace/search and /discover
  in: header
  name: consumerApiKey
  obtain: POST https://rettfrabonden.com/api/keys with optional JSON body {label, contact_email}; the key is returned once and cannot be retrieved again
  parameter: X-API-Key
  required_for: []
  revoke: POST https://rettfrabonden.com/api/keys/revoke (stops the key, keeps history) or POST https://rettfrabonden.com/api/keys/erase (GDPR erasure of label/e-mail); both take {key} in the body or the key as X-API-Key
  role: voluntary consumer-identity key for AI agents
  scopes:
  - read
  sources:
  - a2a/rettfrabonden-com-agent-card.json
  - llms/rettfrabonden-com-llms.txt
  type: apiKey
- description: The only securityScheme declared in /openapi.json, and the scheme that spec attaches to registerProducer. Every other provider document (agent card, protected-resource metadata, server card, /api index, agents.txt) says registration is gated by X-API-Key, not X-Admin-Key. Recorded as spec drift; the privacy page describes admin access as "protected with API keys in environment variables", i.e. an operator credential.
  in: header
  name: adminKey
  parameter: X-Admin-Key
  required_for:
  - admin routes — not part of the public surface
  role: operator/admin key
  scopes: []
  sources:
  - openapi/rettfrabonden-com-agent-surface-openapi.json
  type: apiKey
- applies_to:
  - searchFood
  - searchProducers
  - discoverProducers
  - listProducers
  - getProducerInfo
  - getProducer
  - geocodePlace
  - getAcpProductFeed
  - getPlatformStats
  - getAgentCard
  - every MCP tool
  - A2A message/send
  - tasks/get
  - tasks/list
  description: Anonymous access; rate-limited per IP (see rate-limits/).
  name: none
  sources:
  - openapi/rettfrabonden-com-openapi.yml
  - mcp/rettfrabonden-com-mcp-tools.json
  type: none
slug: rettfrabonden-com-authentication
source_filename: rettfrabonden-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/rettfrabonden-com-agent-surface-openapi.json\ndocs:\n- https://rettfrabonden.com/llms.txt\n- https://rettfrabonden.com/.well-known/agent-card.json\n- https://rettfrabonden.com/.well-known/oauth-protected-resource\n- https://rettfrabonden.com/teknologi\nsummary:\n  types: [apiKey, none]\n  api_key_in: [header]\n  oauth2_flows: []\n  model: >-\n    Reads are open. Every search/discover/detail/geocode/stats operation, the whole MCP tool surface\n    (including the anonymous cart flow) and the A2A message/send and tasks/* methods answer with no\n    credential. The ONE key-gated write is producer registration (POST /api/marketplace/register),\n    which requires an X-API-Key. A second, voluntary X-API-Key — the \"consumer key\" from POST /api/keys —\n    exists only to raise the caller's rate-limit ceiling and to attribute usage; it is not a login.\n    There is no OAuth, no OIDC and no bearer-token issuance: the RFC 9728\
  \ protected-resource document\n    declares authorization_servers [] and names the API key as the credential in vendor x-auth-* fields.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  role: producer key\n  required_for: [registerProducer, producer-side writes documented as \"write operations\"]\n  obtain: 'issued in the response to POST /api/marketplace/register (openapi.json: \"Registered agent with API key\"; protected-resource x-auth-obtain-url)'\n  scopes: [write]\n  sources: [a2a/rettfrabonden-com-agent-card.json, well-known/rettfrabonden-com-oauth-protected-resource.json, well-known/rettfrabonden-com-mcp-server-card.json]\n  description: API key received upon registration. Required for write operations; read/search operations are open.\n- name: consumerApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  role: voluntary consumer-identity key for AI agents\n  required_for: []\n  obtain: POST https://rettfrabonden.com/api/keys with optional\
  \ JSON body {label, contact_email}; the key is returned once and cannot be retrieved again\n  revoke: POST https://rettfrabonden.com/api/keys/revoke (stops the key, keeps history) or POST https://rettfrabonden.com/api/keys/erase (GDPR erasure of label/e-mail); both take {key} in the body or the key as X-API-Key\n  effect: about 3x higher rate-limit ceiling on the general REST and /a2a surface (300 -> 900 and 200 -> 600 per 15 minutes) and a per-key usage ledger (endpoint/tool name and date only); does NOT raise the static 150-per-15-minute quota on /api/marketplace/search and /discover\n  scopes: [read]\n  sources: [a2a/rettfrabonden-com-agent-card.json, llms/rettfrabonden-com-llms.txt]\n  description: Free, voluntary key — same header name as the producer key, different purpose; nothing requires it.\n- name: adminKey\n  type: apiKey\n  in: header\n  parameter: X-Admin-Key\n  role: operator/admin key\n  required_for: [admin routes — not part of the public surface]\n  scopes: []\n  sources:\
  \ [openapi/rettfrabonden-com-agent-surface-openapi.json]\n  description: >-\n    The only securityScheme declared in /openapi.json, and the scheme that spec attaches to registerProducer.\n    Every other provider document (agent card, protected-resource metadata, server card, /api index,\n    agents.txt) says registration is gated by X-API-Key, not X-Admin-Key. Recorded as spec drift; the\n    privacy page describes admin access as \"protected with API keys in environment variables\", i.e. an\n    operator credential.\n- name: none\n  type: none\n  applies_to: [searchFood, searchProducers, discoverProducers, listProducers, getProducerInfo, getProducer, geocodePlace, getAcpProductFeed, getPlatformStats, getAgentCard, every MCP tool, A2A message/send, tasks/get, tasks/list]\n  sources: [openapi/rettfrabonden-com-openapi.yml, mcp/rettfrabonden-com-mcp-tools.json]\n  description: Anonymous access; rate-limited per IP (see rate-limits/).\nobservations:\n- POST /api/marketplace/register with\
  \ an empty JSON body and no key returned HTTP 400 with a zod validation error list, not 401 — input validation runs before (or instead of) the key check on an empty body, so which header actually gates a valid registration could not be observed without submitting a real registration, which this pass did not do.\n- The card carries authentication {schemes:[apiKey]} (pre-0.3 shape) and security [] (no requirement) alongside its securitySchemes map.\n- The site has no OpenID/OAuth discovery documents (/.well-known/openid-configuration and /oauth-authorization-server both 404) — scopes_supported [read, write] in the protected-resource document are API-key scopes, not OAuth scopes, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/authentication/rettfrabonden-com-authentication.yml
summary_line: apiKey/none · 4 schemes
tags:
- Local Food
- Agriculture
- Food
- Marketplace
- Directory
- Search
- Geolocation
- Agent-to-Agent
- MCP
- Norway
- Open-Source
- Company
---
