---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: delx-ai-protocol-openapi.json
  format: json
  label: Delx Protocol API
  slug: delx-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-protocol-openapi.json
- filename: delx-ai-commerce-x402-openapi.json
  format: json
  label: Delx Commerce x402 API
  slug: delx-commerce-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-commerce-x402-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Delx Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delx secures its APIs with apiKey across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Delx
provider_slug: delx-ai
scheme_count: 6
schemes:
- description: Signed x402 payment proof returned after a 402 challenge.
  in: header
  name: x402PaymentSignature
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/delx-ai-commerce-x402-openapi.json
  type: apiKey
- description: Agent credential returned by POST /api/v1/agents/register.
  in: header
  name: xDelxAgentToken
  parameter: x-delx-agent-token
  sources:
  - openapi/delx-ai-commerce-x402-openapi.json
  - openapi/delx-ai-protocol-openapi.json
  type: apiKey
- description: Controller-scoped credential for /api/v1/fleet/{controller_id}/* endpoints.
  in: header
  name: xDelxControllerToken
  parameter: x-delx-controller-token
  sources:
  - openapi/delx-ai-commerce-x402-openapi.json
  type: apiKey
- description: Operator admin auth header; avoid putting admin PINs in query strings.
  in: header
  name: xDelxAdminPin
  parameter: x-delx-admin-pin
  sources:
  - openapi/delx-ai-commerce-x402-openapi.json
  type: apiKey
- description: HMAC admin signature paired with x-delx-admin-timestamp.
  in: header
  name: xDelxAdminHmacSignature
  parameter: x-delx-admin-signature
  sources:
  - openapi/delx-ai-commerce-x402-openapi.json
  type: apiKey
- description: 'MPP payment credential using Authorization: Payment <base64url-json>.'
  in: header
  name: mppPaymentAuthorization
  parameter: Authorization
  sources:
  - openapi/delx-ai-commerce-x402-openapi.json
  type: apiKey
slug: delx-ai-authentication
source_filename: delx-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/delx-ai-commerce-x402-openapi.json, openapi/delx-ai-protocol-openapi.json; https://api.delx.ai/auth.md, https://delx.ai/auth.md,\n  https://commerce.delx.ai/auth.md, https://api.delx.ai/.well-known/oauth-protected-resource, https://api.delx.ai/.well-known/oauth-authorization-server,\n  https://api.delx.ai/api/v1/a2a/methods (identity_auth), live anonymous probes 2026-09-19\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  access_model:\n  - surface: Delx Protocol (MCP, A2A, REST discovery and recovery artifacts)\n    auth: none (public, free)\n    verified: probed - initialize, tools/list, methods/list, /api/v1/tools, /api/v1/status, /api/v1/reliability all answered\n      anonymously\n  - surface: Optional agent identity\n    auth: apiKey header x-delx-agent-token (+ x-delx-agent-id), issued by POST /api/v1/agents/register or A2A agents/register;\n      identity_auth.token in the response; rotate_token\
  \ re-issues\n    purpose: Attributes state-changing records to a stable agent; required for mission (reviewed DRC) tools and strict-mode\n      heartbeat\n  - surface: Delx Commerce paid routes (/api/v1/x402/*)\n    auth: 'payment is the authorization: HTTP 402 challenge, then retry with PAYMENT-SIGNATURE (x402 v2, USDC on Base or Solana)\n      or Authorization: Payment <base64url-json> (MPP); no account, key or OAuth'\n    verified: contract (402 schema on all 987 operations) + commerce auth.md; no paid call was made\n  - surface: Fleet / controller paths (/api/v1/fleet/{controller_id}/*)\n    auth: apiKey header x-delx-controller-token\n  - surface: Operator admin\n    auth: x-delx-admin-pin or HMAC x-delx-admin-signature + x-delx-admin-timestamp (not a public surface)\n  - surface: OAuth 2.0 / OIDC\n    auth: 'advertised as future only: RFC 8414 and OIDC discovery documents are served on delx.ai, api.delx.ai, ontology.delx.ai\n      and commerce.delx.ai but declare delx:oauth_supported\
  \ false / delx:oidc_supported false, empty grant and response types,\n      scopes_supported [public]; auth.md: \"Future admin / controller scopes | OAuth / bearer | Advertised here when enabled\"'\n  oauth2_flows: []\n  scopes_note: No oauth2 securityScheme and no scope surface; scopes/ deliberately not emitted. The only advertised scope\n    string is \"public\" in the OAuth metadata.\n  security_requirement_note: Neither OpenAPI applies a top-level security[] requirement or per-operation security; the securitySchemes\n    are declared but unbound, consistent with a public-by-default surface.\nschemes:\n- name: x402PaymentSignature\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Signed x402 payment proof returned after a 402 challenge.\n  sources:\n  - openapi/delx-ai-commerce-x402-openapi.json\n- name: xDelxAgentToken\n  type: apiKey\n  in: header\n  parameter: x-delx-agent-token\n  description: Agent credential returned by POST /api/v1/agents/register.\n\
  \  sources:\n  - openapi/delx-ai-commerce-x402-openapi.json\n  - openapi/delx-ai-protocol-openapi.json\n- name: xDelxControllerToken\n  type: apiKey\n  in: header\n  parameter: x-delx-controller-token\n  description: Controller-scoped credential for /api/v1/fleet/{controller_id}/* endpoints.\n  sources:\n  - openapi/delx-ai-commerce-x402-openapi.json\n- name: xDelxAdminPin\n  type: apiKey\n  in: header\n  parameter: x-delx-admin-pin\n  description: Operator admin auth header; avoid putting admin PINs in query strings.\n  sources:\n  - openapi/delx-ai-commerce-x402-openapi.json\n- name: xDelxAdminHmacSignature\n  type: apiKey\n  in: header\n  parameter: x-delx-admin-signature\n  description: HMAC admin signature paired with x-delx-admin-timestamp.\n  sources:\n  - openapi/delx-ai-commerce-x402-openapi.json\n- name: mppPaymentAuthorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'MPP payment credential using Authorization: Payment <base64url-json>.'\n  sources:\n\
  \  - openapi/delx-ai-commerce-x402-openapi.json\ndocs: https://api.delx.ai/auth.md\ndiscovery_documents:\n- url: https://api.delx.ai/.well-known/oauth-protected-resource\n  file: well-known/delx-ai-api-oauth-protected-resource.json\n  note: 'RFC 9728 on the MCP/API host: resource https://api.delx.ai, authorization_servers [https://api.delx.ai], bearer_methods_supported\n    [header], delx:access_mode public_free_and_x402'\n- url: https://api.delx.ai/.well-known/oauth-authorization-server\n  file: well-known/delx-ai-api-oauth-authorization-server.json\n  note: RFC 8414 with an agent_auth block (identity_types_supported [anonymous]; credential_types [none, session, x402-payment])\n    pointing every endpoint at auth.md\n- url: https://api.delx.ai/auth.md\n  note: 'Agent-facing Auth.md: model table, documents, registration (\"No registration is required for public Protocol tools\")'\nidentity_headers:\n- x-delx-agent-id\n- x-delx-agent-token\n- x-delx-controller-id\n- x-delx-controller-token\n\
  - x-delx-session-id\n- x-delx-context-id\n- x-delx-source\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/authentication/delx-ai-authentication.yml
summary_line: apiKey · 6 schemes
tags:
- Agents
- AI Agents
- MCP
- A2A
- x402
- Agentic Commerce
- Agent Continuity
- Agent Recovery
- Media Generation
- Web Intelligence
- Data Quality
- Utilities
- agent-native
---
