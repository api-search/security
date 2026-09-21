---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: whisper-online-openapi.json
  format: json
  label: Whisper API
  slug: whisper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-openapi.json
auth_types:
- apiKey
- http-bearer
- oauth2
- network-identity
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Whisper Online Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whisper Security secures its APIs with apiKey, http-bearer, oauth2, and network-identity across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Whisper Security
provider_slug: whisper-online
scheme_count: 5
schemes:
- description: 'A whisper_live_... key (the openapi securityScheme). Obtainable from an email address alone with no human step: POST https://console.whisper.security/api/signup {email} then POST /api/signup/verify {signup_id, code} returns the key (6-digit code, 15-minute TTL, 5 tries). Required only for the control plane (CALL whisper.agents) and the one graph write (submit); every other read answers keyless. The secret is shown once at creation.'
  in: header
  name: whisperApiKey
  parameter: X-API-Key
  sources:
  - openapi/whisper-online-openapi.json
  - https://whisper.online/.well-known/agent-onboarding.json
  type: apiKey
- description: 'On graph.whisper.online / graph.whisper.security the same key is also accepted as Authorization: Bearer <key> or Authorization: ApiKey <key>; X-API-Key is canonical. A missing or unrecognised key does NOT fail the request — it runs with reduced (anonymous) access and answers 200; confirm with CALL whisper.quota() (isAnonymous must be false).'
  name: bearer / ApiKey (graph endpoints)
  scheme: bearer
  sources:
  - https://www.whisper.security/docs/cypher-api/reference
  type: http
- description: 'RFC 9728 protected resource; RFC 7591 dynamic client registration and Client ID Metadata Documents; PKCE S256 only; public clients (token_endpoint_auth_methods_supported [none]); access tokens 1 hour, refresh tokens up to 180 days rotating. Static keys are the fallback as Authorization: Bearer or X-API-Key; a request with no credentials is rejected with 401 (probed 2026-09-19). Detail in scopes/whisper-online-scopes.yml.'
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.whisper.security/oauth/authorize
      refreshUrl: https://mcp.whisper.security/oauth/token
      scopes:
        mcp:query: legacy alias of mcp:read
        mcp:read: the whole read-only surface
        offline_access: refresh token
      tokenUrl: https://mcp.whisper.security/oauth/token
  name: OAuth 2.1 (hosted MCP server)
  sources:
  - https://www.whisper.security/docs/ai/mcp/setup
  - well-known/whisper-online-mcp-oauth-authorization-server.json
  type: oauth2
- description: 'From inside a connected agent, requests to https://[<agent /128>]/api/query and the per-verb GETs (/identify?q=, /assess, /explain ...) carry no key at all: the routable /128 the request originates from IS the credential, and the answer is scoped to that identity. Verifiers check the identity keylessly via reverse DNS + forward AAAA + DANE TLSA (3 1 1) under DNSSEC + RDAP.'
  name: agent-plane address-as-credential
  sources:
  - https://whisper.online/docs/graph-api
  - https://menu.whisper.online/menu
  type: network-identity
- description: CALL whisper.agents({op:'register'}) mints a brand-new agent with its own api_key, "handed back exactly once". op:identity allocates a /128 on the caller's existing key instead.
  in: header
  name: per-agent API key
  parameter: X-API-Key
  sources:
  - https://whisper.online/docs/control-plane
  type: apiKey
slug: whisper-online-authentication
source_filename: whisper-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://whisper.online/docs/control-plane\nderived_from: openapi/whisper-online-openapi.json\ndocs:\n- https://whisper.online/docs/control-plane\n- https://whisper.online/docs/graph-api\n- https://whisper.online/docs/account-and-keys\n- https://whisper.online/.well-known/agent-onboarding.json\n- https://www.whisper.security/docs/ai/agent-signup\n- https://www.whisper.security/docs/ai/mcp/setup\n- https://www.whisper.security/docs/cypher-api/reference\n- https://mcp.whisper.security/.well-known/oauth-authorization-server\nsummary:\n  types: [apiKey, http-bearer, oauth2, network-identity]\n  api_key_in: [header]\n  keyless_tier: true\nschemes:\n- name: whisperApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'A whisper_live_... key (the openapi securityScheme). Obtainable from an email address alone with no human step: POST https://console.whisper.security/api/signup {email} then POST /api/signup/verify\
  \ {signup_id, code} returns the key (6-digit code, 15-minute TTL, 5 tries). Required only for the control plane (CALL whisper.agents) and the one graph write (submit); every other read answers keyless. The secret is shown once at creation.'\n  sources: [openapi/whisper-online-openapi.json, 'https://whisper.online/.well-known/agent-onboarding.json']\n- name: bearer / ApiKey (graph endpoints)\n  type: http\n  scheme: bearer\n  description: 'On graph.whisper.online / graph.whisper.security the same key is also accepted as Authorization: Bearer <key> or Authorization: ApiKey <key>; X-API-Key is canonical. A missing or unrecognised key does NOT fail the request — it runs with reduced (anonymous) access and answers 200; confirm with CALL whisper.quota() (isAnonymous must be false).'\n  sources: ['https://www.whisper.security/docs/cypher-api/reference']\n- name: OAuth 2.1 (hosted MCP server)\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.whisper.security/oauth/authorize\n\
  \      tokenUrl: https://mcp.whisper.security/oauth/token\n      refreshUrl: https://mcp.whisper.security/oauth/token\n      scopes: {mcp:read: the whole read-only surface, offline_access: refresh token, mcp:query: legacy alias of mcp:read}\n  description: 'RFC 9728 protected resource; RFC 7591 dynamic client registration and Client ID Metadata Documents; PKCE S256 only; public clients (token_endpoint_auth_methods_supported [none]); access tokens 1 hour, refresh tokens up to 180 days rotating. Static keys are the fallback as Authorization: Bearer or X-API-Key; a request with no credentials is rejected with 401 (probed 2026-09-19). Detail in scopes/whisper-online-scopes.yml.'\n  sources: ['https://www.whisper.security/docs/ai/mcp/setup', well-known/whisper-online-mcp-oauth-authorization-server.json]\n- name: agent-plane address-as-credential\n  type: network-identity\n  description: 'From inside a connected agent, requests to https://[<agent /128>]/api/query and the per-verb GETs (/identify?q=,\
  \ /assess, /explain ...) carry no key at all: the routable /128 the request originates from IS the credential, and the answer is scoped to that identity. Verifiers check the identity keylessly via reverse DNS + forward AAAA + DANE TLSA (3 1 1) under DNSSEC + RDAP.'\n  sources: ['https://whisper.online/docs/graph-api', 'https://menu.whisper.online/menu']\n- name: per-agent API key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'CALL whisper.agents({op:''register''}) mints a brand-new agent with its own api_key, \"handed back exactly once\". op:identity allocates a /128 on the caller''s existing key instead.'\n  sources: ['https://whisper.online/docs/control-plane']\ncli_key_ladder: 'WHISPER_API_KEY or WHISPER_KEY env, else the credential saved by `whisper login` (browser device-flow at console.whisper.online, or a pasted key); the key travels only in the header, never in the query string or a Cypher literal.'\nconsole: 'https://console.whisper.security (sign-up) /\
  \ https://console.whisper.online (sign-in); the console issues short-lived session tokens for browser use; browser cross-origin calls to the API are refused with 403.'\nmtls_dpop: 'A per-agent CA (Whisper Agent Identity Root CA / Issuing CA, O=viaGraph B.V.; fingerprints at /.well-known/whisper-ca.json), mTLS and DPoP are documented for agent-to-server authentication at /docs/per-agent-ca and /docs/egress-auth; not part of the REST API securitySchemes.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/authentication/whisper-online-authentication.yml
summary_line: apiKey/http-bearer/oauth2/network-identity · 5 schemes
tags:
- Agent Identity
- Agents
- IPv6
- DNS
- DNSSEC
- Threat Intelligence
- Security
- Egress
- A2A
- MCP
- RDAP
- Transparency Log
- Graph Database
- agent-native
- Netherlands
---
