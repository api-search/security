---
anonymous_access: false
api_key_in: []
api_specs:
- filename: relmcrm-com-openapi.yml
  format: yaml
  label: Relm CRM REST API
  slug: relm-crm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/openapi/relmcrm-com-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Relmcrm Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Relm secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Relm
provider_slug: relmcrm-com
scheme_count: 2
schemes:
- at_rest: SHA-256 hash; a lost key is rotated, never recovered (https://relmcrm.com/security)
  description: Workspace-scoped API key. relm_live_... (live) or relm_test_... (free, isolated test mode). Mint at https://app.relmcrm.com/.
  failure: '401 application/problem+json code unauthorized — "Missing or invalid API key. Send `Authorization: Bearer relm_live_...`." (observed live)'
  header: 'Authorization: Bearer <key>'
  key_prefixes:
    live: relm_live_
    test: relm_test_
  minted_at: https://app.relmcrm.com/ (dashboard, "API keys" — live and test tabs)
  name: bearerAuth
  recommended_for: servers and CI (docs); required for test mode
  scheme: bearer
  scoping: workspace-bound; the key decides test vs live mode and data never crosses
  shown_once: true
  sources:
  - openapi/relmcrm-com-openapi.yml
  - https://relmcrm.com/docs
  type: http
- connected_apps: listed in the dashboard; disconnecting revokes all access immediately (changelog v0.17.0)
  consent_screen: names the actual redirect destination and marks the app's self-declared name as unverified; anti-clickjacking protection; account creation and email confirmation inline (changelog v0.13.0–v0.15.0)
  description: 'OAuth 2.1 with PKCE (S256) and dynamic client registration (RFC 7591). Live mode only; test mode is API-key only. Discovery: /.well-known/oauth-authorization-server.'
  discovery:
    authorization_server: https://api.relmcrm.com/.well-known/oauth-authorization-server (well-known/relmcrm-com-oauth-authorization-server.json)
    protected_resource: https://api.relmcrm.com/.well-known/oauth-protected-resource (well-known/relmcrm-com-oauth-protected-resource.json)
  dynamic_client_registration: RFC 7591 at https://api.relmcrm.com/oauth/register (POST; GET returns 404)
  flows:
  - authorizationUrl: https://api.relmcrm.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.relmcrm.com/oauth/token
    scopes: 1
    tokenUrl: https://api.relmcrm.com/oauth/token
  issuer: https://api.relmcrm.com
  live_only: true
  live_only_note: OAuth grants act on live data; test mode stays API-key only (docs).
  name: oauth2
  pkce: S256 required
  recommended_for: end-user chat clients (Claude, ChatGPT) — "the client registers itself, you approve in a browser, and you never handle a secret"
  refresh_tokens: yes, with rotation (docs)
  revocation: https://api.relmcrm.com/oauth/revoke
  see: scopes/relmcrm-com-scopes.yml
  sources:
  - openapi/relmcrm-com-openapi.yml
  - well-known/relmcrm-com-oauth-authorization-server.json
  - https://relmcrm.com/docs
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
  version: OAuth 2.1
slug: relmcrm-com-authentication
source_filename: relmcrm-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/relmcrm-com-openapi.yml (components.securitySchemes bearerAuth + oauth2; root security[]) + https://relmcrm.com/docs (Base URL & auth; Connect via MCP; OAuth 2.1) + https://relmcrm.com/security (Secrets and keys) + well-known/relmcrm-com-oauth-authorization-server.json + live probes 2026-09-19 (401 on GET https://api.relmcrm.com/v1/schema; JSON-RPC -32001 + WWW-Authenticate on anonymous MCP tools/call; failed Task on anonymous A2A message/send)\ndocs: https://relmcrm.com/docs\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  one_credential_three_surfaces: The same bearer key (or OAuth access token) authenticates REST (https://api.relmcrm.com/v1), MCP (https://api.relmcrm.com/mcp) and A2A (https://api.relmcrm.com/a2a).\n  anonymous_surface: MCP initialize and tools/list, the OpenAPI, llms.txt, the agent card, the MCP descriptor and both OAuth discovery documents are public; every data\
  \ operation requires a credential.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <key>'\n  key_prefixes:\n    live: relm_live_\n    test: relm_test_\n  minted_at: https://app.relmcrm.com/ (dashboard, \"API keys\" — live and test tabs)\n  shown_once: true\n  at_rest: SHA-256 hash; a lost key is rotated, never recovered (https://relmcrm.com/security)\n  scoping: workspace-bound; the key decides test vs live mode and data never crosses\n  recommended_for: servers and CI (docs); required for test mode\n  description: Workspace-scoped API key. relm_live_... (live) or relm_test_... (free, isolated test mode). Mint at https://app.relmcrm.com/.\n  failure: >-\n    401 application/problem+json code unauthorized — \"Missing or invalid API key. Send `Authorization: Bearer\n    relm_live_...`.\" (observed live)\n  sources:\n  - openapi/relmcrm-com-openapi.yml\n  - https://relmcrm.com/docs\n- name: oauth2\n  type: oauth2\n  version: OAuth 2.1\n  issuer:\
  \ https://api.relmcrm.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.relmcrm.com/oauth/authorize\n    tokenUrl: https://api.relmcrm.com/oauth/token\n    refreshUrl: https://api.relmcrm.com/oauth/token\n    scopes: 1\n  pkce: S256 required\n  refresh_tokens: yes, with rotation (docs)\n  dynamic_client_registration: RFC 7591 at https://api.relmcrm.com/oauth/register (POST; GET returns 404)\n  revocation: https://api.relmcrm.com/oauth/revoke\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  discovery:\n    authorization_server: https://api.relmcrm.com/.well-known/oauth-authorization-server (well-known/relmcrm-com-oauth-authorization-server.json)\n    protected_resource: https://api.relmcrm.com/.well-known/oauth-protected-resource (well-known/relmcrm-com-oauth-protected-resource.json)\n  live_only: true\n  live_only_note: OAuth grants act on live data; test mode stays API-key only (docs).\n  recommended_for: end-user chat clients\
  \ (Claude, ChatGPT) — \"the client registers itself, you approve in a browser, and you never handle a secret\"\n  consent_screen: names the actual redirect destination and marks the app's self-declared name as unverified; anti-clickjacking protection; account creation and email confirmation inline (changelog v0.13.0–v0.15.0)\n  connected_apps: listed in the dashboard; disconnecting revokes all access immediately (changelog v0.17.0)\n  description: 'OAuth 2.1 with PKCE (S256) and dynamic client registration (RFC 7591). Live mode only; test mode is API-key only. Discovery: /.well-known/oauth-authorization-server.'\n  see: scopes/relmcrm-com-scopes.yml\n  sources:\n  - openapi/relmcrm-com-openapi.yml\n  - well-known/relmcrm-com-oauth-authorization-server.json\n  - https://relmcrm.com/docs\nchallenges_observed:\n- surface: REST\n  request: GET https://api.relmcrm.com/v1/schema (no credential)\n  status: 401\n  body: application/problem+json type https://relmcrm.com/errors/unauthorized\n  www_authenticate:\
  \ not present on the REST 401\n- surface: MCP\n  request: POST https://api.relmcrm.com/mcp tools/call relm_describe_schema (no credential)\n  status: 401\n  body: >-\n    JSON-RPC error -32001 \"Authorization required. Connect with OAuth, or send Authorization: Bearer relm_live_...\"\n  www_authenticate: Bearer realm=\"Relm\", resource_metadata=\"https://api.relmcrm.com/.well-known/oauth-protected-resource\"\n  note: Also mirrored in error.data._meta[\"mcp/www_authenticate\"]; this is the RFC 9728 §5.1 hop that lets an MCP client offer a Connect button.\n- surface: A2A\n  request: POST https://api.relmcrm.com/a2a message/send (no credential)\n  status: 200\n  body: >-\n    terminal Task state failed; agent message text \"Authentication required. Send Authorization: Bearer relm_live_...\n    (or relm_test_...)\"; data part code unauthorized, auth bearer\nmcp_security_schemes_per_tool: >-\n  every one of the 41 tools declares securitySchemes oauth2 with scopes [crm] (mcp/relmcrm-com-mcp-tools-list.json);\n\
  \  the bearer alternative is documented in /.well-known/mcp.json.\nagent_card_security: >-\n  securitySchemes oauth2 (authorizationCode, scope crm) + bearer (http); security requires oauth2 [crm] OR bearer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relmcrm-com/refs/heads/main/authentication/relmcrm-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- CRM
- Sales
- Contacts
- Deals
- Sales Pipeline
- Automation
- Webhook
- MCP
- A2A
- AI Agents
- Agent-Native
- United Arab Emirates
---
