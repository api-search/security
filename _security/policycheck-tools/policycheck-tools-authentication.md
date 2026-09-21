---
anonymous_access: true
api_key_in: []
api_specs:
- filename: policycheck-tools-openapi.yml
  format: yaml
  label: PolicyCheck API
  slug: policycheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/policycheck-tools/refs/heads/main/openapi/policycheck-tools-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Policycheck Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: PolicyCheck declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: PolicyCheck
provider_slug: policycheck-tools
scheme_count: 3
schemes:
- applies_to:
  - POST /api/check
  - POST /api/a2a
  - GET /api/clause-registry
  - POST /api/v1/signed-assessment
  - POST /api/v1/verify
  - GET /.well-known/jwks.json
  - POST /api/chatgpt/analyze (OpenAPI analyzeLegalDocument)
  - POST /api/chatgpt/analyze-url (OpenAPI analyzeLegalDocumentFromURL)
  evidence:
  - POST /api/check {} -> 400 {"error":"Provide seller_url (or url) or policy_text"} (not 401)
  - POST /api/v1/signed-assessment {} -> 400 {"error":"Provide seller_url (or url) or policy_text (or text)"} (not 401)
  - POST /api/a2a tasks/get -> 200 JSON-RPC error -32001 (served without a key)
  - 'POST /api/chatgpt/analyze {} -> 400 {"error":"Missing required field: text"}'
  - ai-plugin.json auth.type = none
  id: anonymous
  note: 'X-API-Key is OPTIONAL on /api/v1/signed-assessment: the homepage example sends it so the check is attributed to the caller''s audit trail (with agent_id and transaction_ref), but the endpoint answers without it.'
  type: none
- applies_to:
  - GET /api/v1/audit-log
  - GET /api/v1/compliance-report
  - POST /api/v1/signed-assessment (optional; attributes the check to your audit trail)
  evidence:
  - GET /api/v1/audit-log -> 401 {"error":"X-API-Key header required"}; no WWW-Authenticate header
  - 'agent card securitySchemes.apiKey: type apiKey, in header, name X-API-Key'
  id: apiKey
  in: header
  key_format: undocumented
  key_issuance:
    contact: api@policycheck.tools
    note: 'Agent card: "Free tier: 100 requests/minute. Contact api@policycheck.tools for higher limits." No docs page explains how to obtain a key.'
    self_serve: false
    signup_url: null
  name: X-API-Key
  type: apiKey
- applies_to:
  - POST /api/x402/analyze
  evidence:
  - POST /api/x402/analyze {} -> 402 with PAYMENT-REQUIRED header (x402Version 2, $0.03 USDC on Base)
  id: x402
  in: header
  name: X-PAYMENT
  note: Payment-gated, not identity-gated; see x402/policycheck-tools-x402.yml.
  type: payment
slug: policycheck-tools-authentication
source_filename: policycheck-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://policycheck.tools/docs\ndocs:\n- https://policycheck.tools/docs#rate-limits\n- https://policycheck.tools/.well-known/agent.json\n- https://policycheck.tools/llms.txt\nderived_from: openapi/policycheck-tools-openapi.yml\nsummary: >-\n  PolicyCheck is anonymous by default: the primary analysis endpoints (/api/check, /api/a2a, /api/clause-registry,\n  /api/v1/signed-assessment, /api/v1/verify, /.well-known/jwks.json) accept requests with no credential, and the\n  published OpenAPI declares no securitySchemes at all. Two account-scoped endpoints — /api/v1/audit-log and\n  /api/v1/compliance-report — require an X-API-Key header (live 401 \"X-API-Key header required\" without one), and\n  the paid /api/x402/analyze endpoint is gated by payment (HTTP 402) rather than identity. The agent card declares\n  a blanket X-API-Key requirement that the live free endpoints do not enforce. No signup or key-issuance page\n  exists; the\
  \ only published route to a key is the agent card's \"Contact api@policycheck.tools for higher limits\".\nschemes:\n- id: anonymous\n  type: none\n  applies_to:\n  - POST /api/check\n  - POST /api/a2a\n  - GET /api/clause-registry\n  - POST /api/v1/signed-assessment\n  - POST /api/v1/verify\n  - GET /.well-known/jwks.json\n  - POST /api/chatgpt/analyze (OpenAPI analyzeLegalDocument)\n  - POST /api/chatgpt/analyze-url (OpenAPI analyzeLegalDocumentFromURL)\n  evidence:\n  - 'POST /api/check {} -> 400 {\"error\":\"Provide seller_url (or url) or policy_text\"} (not 401)'\n  - 'POST /api/v1/signed-assessment {} -> 400 {\"error\":\"Provide seller_url (or url) or policy_text (or text)\"} (not 401)'\n  - 'POST /api/a2a tasks/get -> 200 JSON-RPC error -32001 (served without a key)'\n  - 'POST /api/chatgpt/analyze {} -> 400 {\"error\":\"Missing required field: text\"}'\n  - 'ai-plugin.json auth.type = none'\n  note: >-\n    X-API-Key is OPTIONAL on /api/v1/signed-assessment: the homepage example\
  \ sends it so the check is attributed\n    to the caller's audit trail (with agent_id and transaction_ref), but the endpoint answers without it.\n- id: apiKey\n  type: apiKey\n  in: header\n  name: X-API-Key\n  applies_to:\n  - GET /api/v1/audit-log\n  - GET /api/v1/compliance-report\n  - POST /api/v1/signed-assessment (optional; attributes the check to your audit trail)\n  evidence:\n  - 'GET /api/v1/audit-log -> 401 {\"error\":\"X-API-Key header required\"}; no WWW-Authenticate header'\n  - 'agent card securitySchemes.apiKey: type apiKey, in header, name X-API-Key'\n  key_issuance:\n    self_serve: false\n    signup_url: null\n    contact: api@policycheck.tools\n    note: 'Agent card: \"Free tier: 100 requests/minute. Contact api@policycheck.tools for higher limits.\" No docs page explains how to obtain a key.'\n  key_format: undocumented\n- id: x402\n  type: payment\n  in: header\n  name: X-PAYMENT\n  applies_to:\n  - POST /api/x402/analyze\n  evidence:\n  - 'POST /api/x402/analyze\
  \ {} -> 402 with PAYMENT-REQUIRED header (x402Version 2, $0.03 USDC on Base)'\n  note: Payment-gated, not identity-gated; see x402/policycheck-tools-x402.yml.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nprotected_resource_metadata: false\ndynamic_client_registration: false\ndelegated_identity: false\nin_spec:\n  security_schemes_declared: false\n  note: >-\n    The published OpenAPI declares no components.securitySchemes and no security requirement, which is accurate\n    for the two anonymous operations it contains but leaves the X-API-Key endpoints entirely outside the\n    contract. derive-authentication.py therefore produced nothing; this profile is built from the docs, the\n    agent card and live probes.\ngaps:\n- No self-serve key issuance; no documented key format, rotation or revocation.\n- The agent card says every call needs X-API-Key; the docs and the live endpoints say the analysis surface is free and anonymous. Agents that trust the card will stall on a credential\
  \ they cannot obtain.\n- No WWW-Authenticate challenge on the 401, so a client cannot discover the scheme from the response.\n- No OAuth, OIDC or RFC 9728 metadata anywhere (all /.well-known discovery paths 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/policycheck-tools/refs/heads/main/authentication/policycheck-tools-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Policy Analysis
- Consumer Protection
- E-Commerce
- Agentic Commerce
- Risk Assessment
- AI Agents
- A2A
- MCP
- x402
- Legal
- Returns
---
