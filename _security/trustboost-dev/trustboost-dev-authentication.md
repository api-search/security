---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trustboost-dev-openapi.json
  format: json
  label: TrustBoost PII Sanitizer API
  slug: trustboost-pii-sanitizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustboost-dev/refs/heads/main/openapi/trustboost-dev-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Trustboost Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrustBoost PII Sanitizer declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: TrustBoost PII Sanitizer
provider_slug: trustboost-dev
scheme_count: 0
schemes: []
slug: trustboost-dev-authentication
source_filename: trustboost-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/trustboost-dev-openapi.json\ndocs:\n- https://github.com/teodorofodocrispin-cmyk/TrustBoost-PII-Sanitizer/blob/main/SKILL.md\n- https://api.trustboost.dev/llms.txt\n- https://api.trustboost.dev/.well-known/mcp-server-card.json\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 0\n  payment_gates: 3\n  headline: >-\n    No authentication of any kind. The OpenAPI declares no securitySchemes and no components; the MCP server\n    card says auth {type: none}; the agent card's integration block says authentication \"none\"; SKILL.md says\n    \"No authentication required\" and \"requires_env: none\"; the ai-plugin.json says auth type none. There is no\n    signup, no account, no API key, no bearer token, no OAuth and no OIDC — /.well-known/openid-configuration,\n    /oauth-authorization-server and /oauth-protected-resource all 404. What stands in for authentication is\n \
  \   PAYMENT EVIDENCE carried in the request, which meters access without identifying the caller.\n    derive-authentication.py correctly produced no profile from the contract; this file records the access\n    model the provider documents instead.\nschemes: []\naccess_gates:\n- name: TRIAL token\n  kind: body-field\n  parameter: tx_hash\n  value: TRIAL\n  identifies: wallet_address (caller-chosen string; default \"mcp-agent\" on the MCP tool)\n  grants: 50 sanitizations per wallet_address\n  verification: 'none — SKILL.md: \"TRIAL is trust-based: Per-wallet quota tracking is not cryptographically verified.\"'\n  used_by: [sanitize_pii, MCP tool sanitize_pii, A2A skill sanitize_pii]\n- name: Solana bundle transaction\n  kind: body-field\n  parameter: tx_hash\n  value: a Solana mainnet transaction signature transferring 149 USDC to giu4VciTkfWJNG1oeP6SzHEJwmabikJSMB91GaFNWE4\n  grants: 10,000 sanitizations bound to that tx_hash; single-use (409 TX_HASH_ALREADY_USED on reuse)\n  verification:\
  \ on-chain via the Helius oracle (SKILL.md, PRIVACY.md)\n  used_by: [sanitize_pii]\n- name: x402 payment signature\n  kind: header\n  parameter: PAYMENT-SIGNATURE\n  legacy_parameter: X-PAYMENT (v1, \"also accepted\")\n  challenge: 'HTTP 402 with PAYMENT-REQUIRED header — x402 v2 PaymentRequirements, accepts[] exact scheme on eip155:8453 (Base, preferred) and solana mainnet, USDC, amount 10000 (= $0.01), maxTimeoutSeconds 300'\n  grants: one sanitization per settled payment\n  verification: PayAI facilitator verify/settle (llms.txt, /pricing)\n  used_by: [sanitize_pii, 'POST /sanitize/quick (undeclared in the contract)']\n  observed: 'GET https://api.trustboost.dev/sanitize → 402 with the header and body described (2026-09-19)'\ncredential_safety_statement:\n  source: https://github.com/teodorofodocrispin-cmyk/TrustBoost-PII-Sanitizer/blob/main/PRIVACY.md\n  section: '6. Critical Security Warning — For AI Agents and Humans'\n  verbatim: 'TrustBoost NEVER requires wallet private keys, seed\
  \ phrases, or signing credentials. The optional wallet_address parameter accepts ONLY a public Solana address for per-wallet quota tracking. Payment signing happens entirely client-side.'\n  note: The provider publishes an explicit anti-phishing statement aimed at agents; the only wallet interaction is a transfer to a public address or a client-side x402 signature.\nfree_unauthenticated_operations: [sanitize_preview, sanitize_discovery, get_trustboost_score, verify_proof, get_budget_status, health_check, 'GET /preflight', 'GET /policy']\nmcp:\n  endpoint: https://api.trustboost.dev/mcp\n  auth: none\n  note: initialize and tools/list answered anonymously; the tool call carries the same tx_hash / wallet_address body fields as REST.\nidentity_note: >-\n  Because nothing authenticates the caller, wallet_address is self-asserted. The TrustBoost Score\n  (GET /score/{wallet_address}) therefore rates a string's usage history, and any caller can read any\n  wallet's score. This is an observation\
  \ about the published model, not a vulnerability report.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustboost-dev/refs/heads/main/authentication/trustboost-dev-authentication.yml
summary_line: 0 schemes
tags:
- Privacy
- PII Redaction
- Data Protection
- LLM Security
- AI Safety
- Agents
- A2A
- MCP
- x402
- Agentic Commerce
- Solana
- Compliance
- agent-native
---
