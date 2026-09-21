---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kgninja-dev-openapi.json
  format: json
  label: Agent Verification Utility API
  slug: agent-verification-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kgninja-dev/refs/heads/main/openapi/kgninja-dev-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kgninja Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: KG-NINJA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KG-NINJA
provider_slug: kgninja-dev
scheme_count: 1
schemes:
- agent_auth_advertisement: '{"agent_auth":{"skill":"anonymous","register_uri":"https://agent-economy.kgninja.dev/agent/register","identity_types_supported":["anonymous"],"anonymous":{"credential_types_supported":["urn:kgninja:params:agent-credential:anonymous-registration-receipt"],"claim_uri":"https://agent-economy.kgninja.dev/agent/registration"}}}'
  applies_to:
  - getAnonymousAgentRegistration
  bearerFormat: signed anonymous registration receipt
  credential_type: urn:kgninja:params:agent-credential:anonymous-registration-receipt
  description: Optional 15-minute service-local receipt used only to inspect its own registration claim. It grants no API access and does not authorize payment.
  lifetime: 15 minutes
  name: agentRegistration
  observed: 'GET /agent/registration without a bearer -> 401 {"error":{"code":"AGENT_REGISTRATION_REQUIRED","message":"Provide the short-lived registration credential as Authorization: Bearer <credential>.",...}}'
  obtained_by: POST /agent/register with Content-Type application/json and body {} — no email, account, API key or human contact; the response returns the signed credential once
  revocation: none — "There is no revocation endpoint because the receipt has no application privileges and expires after 15 minutes; discard it to stop using it."
  scheme: bearer
  sources:
  - openapi/kgninja-dev-openapi.json
  - https://agent-economy.kgninja.dev/auth.md
  type: http
slug: kgninja-dev-authentication
source_filename: kgninja-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/kgninja-dev-openapi.json\ndocs: https://agent-economy.kgninja.dev/auth.md\nderived_baseline: 'derive-authentication.py 2026-09-19 — 1 scheme (http bearer agentRegistration); upgraded here from the provider''s auth.md and the x402 manifest.'\nsummary:\n  types:\n  - http\n  model: anonymous-by-design; payment (x402) authorizes the one paid operation per request\n  api_key_in: []\n  oauth2_flows: []\n  oidc: false\n  credentials_required_for: [GET /agent/registration only]\n  credentials_not_required_for: [discovery, documentation, health, stats, revenue goal, POST /validate-request, POST /quote, MCP initialize and tools/list, the four free MCP tools, A2A GetTask/ListTasks and the quote-preparation skill]\naccess_model:\n  statement: >-\n    \"The verification service is intentionally anonymous: account registration, an API key, OAuth, OpenID\n    Connect, cookies, and a login session are not required for discovery, quotes,\
  \ or paid execution.\"\n    (auth.md)\n  oauth_metadata: >-\n    \"OAuth authorization-server and protected-resource metadata are intentionally not published because this\n    is not an OAuth-protected resource. The optional anonymous registration receipt is not an OAuth access\n    token.\" — corroborated: /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\n    and /.well-known/openid-configuration all 404 (well-known/kgninja-dev-well-known.yml).\n  delegated_identity: none — no authorization_code flow, no user context; the caller is the paying wallet\n  dynamic_client_registration: none in the RFC 7591 sense; see optional anonymous registration below\nschemes:\n- name: agentRegistration\n  type: http\n  scheme: bearer\n  bearerFormat: signed anonymous registration receipt\n  description: Optional 15-minute service-local receipt used only to inspect its own registration claim. It grants no API access and does not authorize payment.\n  applies_to: [getAnonymousAgentRegistration]\n\
  \  obtained_by: 'POST /agent/register with Content-Type application/json and body {} — no email, account, API key or human contact; the response returns the signed credential once'\n  credential_type: 'urn:kgninja:params:agent-credential:anonymous-registration-receipt'\n  lifetime: 15 minutes\n  revocation: 'none — \"There is no revocation endpoint because the receipt has no application privileges and expires after 15 minutes; discard it to stop using it.\"'\n  observed: 'GET /agent/registration without a bearer -> 401 {\"error\":{\"code\":\"AGENT_REGISTRATION_REQUIRED\",\"message\":\"Provide the short-lived registration credential as Authorization: Bearer <credential>.\",...}}'\n  agent_auth_advertisement: '{\"agent_auth\":{\"skill\":\"anonymous\",\"register_uri\":\"https://agent-economy.kgninja.dev/agent/register\",\"identity_types_supported\":[\"anonymous\"],\"anonymous\":{\"credential_types_supported\":[\"urn:kgninja:params:agent-credential:anonymous-registration-receipt\"],\"claim_uri\"\
  :\"https://agent-economy.kgninja.dev/agent/registration\"}}}'\n  sources:\n  - openapi/kgninja-dev-openapi.json\n  - https://agent-economy.kgninja.dev/auth.md\npayment_authorization:\n  note: Not a securityScheme in the OpenAPI, but the gate that actually protects the paid operation. Recorded here because an agent choosing a credential strategy needs it next to the auth model.\n  protocol: x402 v2 (scheme exact)\n  applies_to: [verifyEvidence, mcp:verify_evidence]\n  precondition: a free precheck receipt digest (POST /validate-request) inside the unchanged paid intent; otherwise 409 PRECHECK_REQUIRED before any quote or 402\n  challenge: HTTP 402 with PAYMENT-REQUIRED header + X402PaymentRequired body; over MCP a tool error with _meta[\"x402/error\"]\n  proof: PAYMENT-SIGNATURE request header (REST) or _meta[\"x402/payment\"] (MCP) on the identical retry\n  settlement_receipt: PAYMENT-RESPONSE header (REST) or _meta[\"x402/payment-response\"] (MCP)\n  terms: 10000 atomic USDC on eip155:8453\
  \ to 0x4D7d842536De9Eb491AE2300126B3CDdE7B0aDE3, asset 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, maxTimeoutSeconds 300 (well-known/kgninja-dev-x402.json)\n  scope_of_the_signature: '\"The x402 signature authorizes only the advertised payment and request. It is not a reusable application credential, is independent of optional agent registration, and does not create an authenticated session.\"'\n  binding: the signed payload must carry the same binding digest as the bound quote; \"A paid retry is accepted only when discovery survived into the paid call and the x402 payload contains the same binding digest.\"\n  operator_identity: Cloudflare Wallet handle @kgninja (https://cloudflare.pay/?handle=kgninja) — public identity of the payee, not a credential the caller uses\ncredential_handling_guidance:\n  verbatim:\n  - 'Never send seed phrases, wallet private keys, API secrets, third-party bearer tokens, or unrelated personal data. Send this service''s short-lived registration receipt only\
  \ to its documented claim endpoint.'\n  - 'Evidence must be bounded inline JSON. The service does not fetch caller-supplied URLs or execute caller code.'\n  - 'Verify returned evidence with https://agent-economy.kgninja.dev/.well-known/jwks.json.'\nverification_keys:\n  jwks: https://agent-economy.kgninja.dev/.well-known/jwks.json\n  file: well-known/kgninja-dev-jwks.json\n  purpose: 'Verifying the service''s Ed25519 evidence signatures (the service signs; callers verify). Not an authentication credential.'\nmcp_registry_proof:\n  url: https://agent-economy.kgninja.dev/.well-known/mcp-registry-auth\n  observed: 'v=MCPv1; k=ed25519; p=<public key>'\n  purpose: domain-ownership proof for MCP Registry publication; public key only\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kgninja-dev/refs/heads/main/authentication/kgninja-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Verification
- JSON
- Cryptography
- Cloudflare Workers
- agent-native
- Japan
---
