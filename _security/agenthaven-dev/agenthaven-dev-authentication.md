---
anonymous_access: true
api_key_in: []
auth_types:
- none
- http-bearer-jwt
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agenthaven Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Bench secures its APIs with none and http-bearer-jwt across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agent Bench
provider_slug: agenthaven-dev
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: '"Needed for create_checkout only; search_flights and tools/list are open. There is no public token endpoint. Two forms are accepted. (1) Sign each call as a request envelope (Authorization: Bearer <compact JWS, typ request+jwt>) under a key attested at /.well-known/agent-keys.json on your own domain, and present at checkout a mandate from an authority this merchant trusts (https://sealedby.dev), bound to the quote and to that key. (2) A JWT issued by this merchant''s operator on request: iss agent-bench-demo-issuer, aud agent-bench, scope commerce:purchase, with a spending cap in EUR."'
  forms:
  - how: Per-call compact JWS with typ request+jwt in the Authorization header, signed by the caller's own key.
    id: request-envelope
    key_attestation: The signing key is attested at /.well-known/agent-keys.json on the CALLER's domain (the merchant does not serve one for itself; travel.agenthaven.dev/.well-known/agent-keys.json 404).
    mandate: At checkout, mandate_jws (typ mandate+jwt) from a trusted authority — GET /health lists mandate_issuers ["https://sealedby.dev"] — bound to quote_hash and to the envelope key; ledger entries record mandate_format ap2-v0.2.
  - how: A JWT the merchant's operator issues on request (no self-service path). Claims stated by the card — iss agent-bench-demo-issuer, aud agent-bench, scope commerce:purchase, plus an EUR spending cap.
    id: operator-issued-jwt
  - how: 'Documented on the page under "Buying as a guest": a buyer with no introduction publishes a P-256 public key in a DNSSEC-signed TXT record at _agent-keys.<its domain> ("v=agentkey1; kty=EC; crv=P-256; x=...; y=..."), signs each call as a request envelope with iss spiffe://<its domain>/<any path>, and presents a mandate it issues itself (typ mandate+jwt, iss https://<its domain>, signed by a key in that record, bound to the quote and the envelope key, living at most 10 minutes).'
    id: guest-buyer
    limits: 'GET /health guests: accepted true, ceiling_minor 100000 EUR (1000.00 EUR per purchase), mandate_max_seconds 600, purchases_per_day 20 (all guests together); guest searches spend the anonymous budget. Contract, vector and a one-file reference buyer at https://provedby.dev/contracts/guest-buyer.md (200, third-party host named by the provider).'
  name: bearer
  required_for:
  - create_checkout
  scheme: bearer
  scopes:
  - commerce:purchase
  sources:
  - a2a/agenthaven-dev-agent-card.json#securitySchemes.bearer
  - a2a/agenthaven-dev-agent-card.json#skills[1].security
  type: http
- applies_to:
  - search_flights
  - tools/list
  - initialize
  - ping
  - /health
  - /ledger
  - well-known documents
  limits: anonymous searches 40 per day and 120 per month, shared; an authorised search never counts (docs; live counters in GET /health counters.anonymous_searches).
  name: anonymous
  sources:
  - https://travel.agenthaven.dev/
  - https://travel.agenthaven.dev/health
  type: none
slug: agenthaven-dev-authentication
source_filename: agenthaven-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://travel.agenthaven.dev/.well-known/agent-card.json\ndocs:\n- https://travel.agenthaven.dev/\n- https://provedby.dev/contracts/guest-buyer.md\nderived_from:\n- a2a/agenthaven-dev-agent-card.json (securitySchemes, skills[].security)\n- mcp/agenthaven-dev-mcp-tools.json (create_checkout inputSchema mandate_jws)\n- https://travel.agenthaven.dev/health (guests policy, mandate_issuers)\nnote: >-\n  derive-authentication.py was not run because the provider publishes no OpenAPI; the profile below is read\n  from the agent card's securitySchemes (the only machine-readable auth declaration), the MCP initialize\n  instructions (which repeat it verbatim), the documentation page, and the live /health document.\nsummary:\n  types: [none, http-bearer-jwt]\n  api_key_in: []\n  oauth2_flows: []\n  token_endpoint: none published\n  discovery: none (no RFC 8414 / OIDC / RFC 9728 documents on any host)\n  anonymous_surface: [MCP initialize,\
  \ MCP ping, MCP tools/list, MCP tools/call search_flights, A2A message/send search_flights, GET /health, GET /ledger, every /.well-known document]\n  authenticated_surface: [MCP tools/call create_checkout, A2A message/send create_checkout]\n  delegation_model: >-\n    Buyer-side mandates rather than OAuth authorization_code. The docs state the checkout token \"carries a\n    spending cap, a currency and a deadline set by the buyer's human; a request above the cap is refused, and\n    the refusal is written to the ledger\" — a delegated, human-bounded authority — but it is expressed as a\n    JWT mandate from an issuer the merchant trusts, not as a token obtained through an authorization server, so\n    no discovery document exists for the rubric's delegated_identity check to read.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  required_for: [create_checkout]\n  scopes: [commerce:purchase]\n  sources: ['a2a/agenthaven-dev-agent-card.json#securitySchemes.bearer',\
  \ 'a2a/agenthaven-dev-agent-card.json#skills[1].security']\n  description: >-\n    \"Needed for create_checkout only; search_flights and tools/list are open. There is no public token endpoint.\n    Two forms are accepted. (1) Sign each call as a request envelope (Authorization: Bearer <compact JWS, typ\n    request+jwt>) under a key attested at /.well-known/agent-keys.json on your own domain, and present at\n    checkout a mandate from an authority this merchant trusts (https://sealedby.dev), bound to the quote and to\n    that key. (2) A JWT issued by this merchant's operator on request: iss agent-bench-demo-issuer, aud\n    agent-bench, scope commerce:purchase, with a spending cap in EUR.\"\n  forms:\n  - id: request-envelope\n    how: Per-call compact JWS with typ request+jwt in the Authorization header, signed by the caller's own key.\n    key_attestation: 'The signing key is attested at /.well-known/agent-keys.json on the CALLER''s domain (the merchant does not serve one for itself;\
  \ travel.agenthaven.dev/.well-known/agent-keys.json 404).'\n    mandate: 'At checkout, mandate_jws (typ mandate+jwt) from a trusted authority — GET /health lists mandate_issuers [\"https://sealedby.dev\"] — bound to quote_hash and to the envelope key; ledger entries record mandate_format ap2-v0.2.'\n  - id: operator-issued-jwt\n    how: A JWT the merchant's operator issues on request (no self-service path). Claims stated by the card — iss agent-bench-demo-issuer, aud agent-bench, scope commerce:purchase, plus an EUR spending cap.\n  - id: guest-buyer\n    how: >-\n      Documented on the page under \"Buying as a guest\": a buyer with no introduction publishes a P-256 public\n      key in a DNSSEC-signed TXT record at _agent-keys.<its domain> (\"v=agentkey1; kty=EC; crv=P-256; x=...;\n      y=...\"), signs each call as a request envelope with iss spiffe://<its domain>/<any path>, and presents a\n      mandate it issues itself (typ mandate+jwt, iss https://<its domain>, signed by a key in\
  \ that record,\n      bound to the quote and the envelope key, living at most 10 minutes).\n    limits: 'GET /health guests: accepted true, ceiling_minor 100000 EUR (1000.00 EUR per purchase), mandate_max_seconds 600, purchases_per_day 20 (all guests together); guest searches spend the anonymous budget. Contract, vector and a one-file reference buyer at https://provedby.dev/contracts/guest-buyer.md (200, third-party host named by the provider).'\n- name: anonymous\n  type: none\n  applies_to: [search_flights, tools/list, initialize, ping, /health, /ledger, well-known documents]\n  limits: anonymous searches 40 per day and 120 per month, shared; an authorised search never counts (docs; live counters in GET /health counters.anonymous_searches).\n  sources: [https://travel.agenthaven.dev/, https://travel.agenthaven.dev/health]\nverification_keys:\n  merchant_jwks: https://travel.agenthaven.dev/.well-known/jwks.json\n  merchant_jwks_note: 'Documented as \"Authorization key set — public keys\
  \ the merchant verifies buyer tokens against\" (kid eF_VZyTpOBYDR0TXuvJF0nALLjaWIHQYWQhgbPZzMnM, ES256).'\n  instance_svid: https://travel.agenthaven.dev/.well-known/spiffe-svid.json\n  trust_bundle: https://travel.agenthaven.dev/.well-known/spiffe-bundle.json\n  dns_aid_record_key: https://dns-aid.agenthaven.dev/.well-known/dns-aid-jwks.json\nrefusals: See errors/agenthaven-dev-problem-types.yml — authorization_missing, authorization_invalid, authorization_denied, signer_unknown, identity_revoked, mandate_expired, mandate_consumed, mandate_revoked and quote_hash_mismatch are the auth-stage refusal reasons observed in the public ledger.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agenthaven-dev/refs/heads/main/authentication/agenthaven-dev-authentication.yml
summary_line: none/http-bearer-jwt · 2 schemes
tags:
- Agents
- A2A
- MCP
- Agentic Commerce
- DNS-AID
- Travel
- Flights
- Payments
- Agent Identity
- Proof of Concept
- agent-native
---
