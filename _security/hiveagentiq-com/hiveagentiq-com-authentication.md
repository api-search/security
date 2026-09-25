---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hiveagentiq-com-hivetrust-openapi.json
  format: json
  label: HiveTrust KYA Identity & Trust API
  slug: hivetrust-kya-identity-trust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivetrust-openapi.json
- filename: hiveagentiq-com-hivegate-openapi.json
  format: json
  label: HiveGate Admission, Identity & Pricing Tier API
  slug: hivegate-admission-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivegate-openapi.json
- filename: hiveagentiq-com-hivebank-openapi.json
  format: json
  label: HiveBank Treasury Attestation & Settlement API
  slug: hivebank-treasury-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivebank-openapi.json
- filename: hiveagentiq-com-hivelaw-openapi.json
  format: json
  label: HiveLaw AI Legal Contracts & Compliance API
  slug: hivelaw-legal-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/openapi/hiveagentiq-com-hivelaw-openapi.json
auth_types:
- apiKey
- http-bearer
- payment
- signature
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Hiveagentiq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hive Agent IQ secures its APIs with apiKey, http-bearer, payment, and signature across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hive Agent IQ
provider_slug: hiveagentiq-com
scheme_count: 6
schemes:
- description: '"Authentication via X-API-Key header" (hivetrust README); examples use ht_your_api_key. The key is issued with the DID at onboarding ("returns a did:hive:* identifier + API key" — thehiveryiq.com/onboard.html; "DID issuance, API key provisioning" — HiveGate ai-plugin.json). The MCP manifest states "tools_list: public, tools_call: X-API-Key or Authorization: Bearer did:hive:* required".'
  in: header
  issuance:
    cost: free for the first DID; premium sovereign DID $4.99 (llms.txt) or $9.99 (402 envelope)
    operation: POST https://hivegate.hiveagentiq.com/v1/gate/onboard
    signup: agent_name + email in the request body (402 envelope quick_start)
  name: HiveDIDApiKey
  parameter: X-API-Key
  sources:
  - https://github.com/srotzin/hivetrust#api-reference
  - https://hivetrust.hiveagentiq.com/.well-known/mcp.json
  - https://hivegate.hiveagentiq.com/.well-known/hivegate.json
  type: apiKey
- bearer_format: did:hive:* (agent DID) or hgate_* (HiveGate guest access token)
  description: 'hivegate.json authentication.methods lists "Authorization: Bearer did:hive:*" and "Authorization: Bearer hgate_*"; the HiveTrust MCP server''s initialize instructions say tools/call for write operations requires "a registered Hive DID via X-API-Key or Authorization: Bearer did:hive:* header". The hgate_ token is returned by hivegate_register_guest / POST /v1/gate/register-guest and is required by hivegate_execute (access_token, "Guest access token (hgate_*)").'
  name: HiveDIDBearer
  scheme: bearer
  sources:
  - https://hivegate.hiveagentiq.com/.well-known/hivegate.json
  - mcp/hiveagentiq-com-hivegate-mcp-tools.json
  type: http
- aliases:
  - x-hive-did
  - x-did
  - X-HiveTrust-DID
  description: 'The "sovereign handshake": "present X-Hive-DID header on non-free endpoints" (HiveGate llms.txt); the 402 envelope lists headers_required ["X-Hive-DID"] and says "After checkout, include your issued did:hive: in the X-Hive-DID header on every request". hivegate.json also names x-did and X-HiveTrust-DID. The same header claims the first-call-free offer ("New here? Add header ''x-hive-did'' to claim your first call free" — agent card bogo block).'
  in: header
  name: HiveDIDHeader
  parameter: X-Hive-DID
  sources:
  - https://hivegate.hiveagentiq.com/llms.txt
  - a2a/hiveagentiq-com-agent-card.json
  type: apiKey
- description: 'Every paid route answers 402. Observed on HiveGate: {"error":"payment_required","code":"HIVE_402", "detail":{"x402": {"version":"1.0","amount_usdc":9.99,"payment_methods":["stripe-checkout","x402-usdc","x402-aleo"],"headers_required": ["X-Hive-DID"]}}}. The HiveGate hive-payments.json names the header: "x402": {"supported": true, "header": "X-Payment", "currency": "USDC", "network": "base"}. llms.txt: "Paid surfaces return a 402 with amount_min_usd — the floor price. Submit any value >= that floor." Settlement rails: USDC/USDT on Base to treasury 0x15184Bf50B3d3F52b60434f8942b7D52F2eB436E, USDC on Solana, USDCx/USAD/ALEO on Aleo. The hivetrust ai-plugin.json declares auth.type "none" with a payment block — payment, not a credential, is the gate.'
  in: header
  name: x402Payment
  observed:
  - code: HIVE_402
    http_status: 402
    url: https://hivegate.hiveagentiq.com/v1/gate/adapters
  - code: HIVE_402
    http_status: 402
    url: https://hivegate.hiveagentiq.com/docs
  parameter: X-Payment
  sources:
  - well-known/hiveagentiq-com-hivegate-hive-payments.json
  - https://hivegate.hiveagentiq.com/llms.txt
  standard: x402 (HTTP 402)
  type: payment
- description: 'All four OpenAPIs carry x-mpp: {realm, payment: {method: tempo, currency: 0x20c0…b50, decimals: 6, recipient}, rails: [x402, mpp]} and per-operation x-mpp-charge {amount, intent: charge} in 6-decimal USDC units ($0.10 = "100000"). No MPP challenge was observed live; recorded from the contract only.'
  name: MPPPayment
  sources:
  - openapi/hiveagentiq-com-hivetrust-openapi.json
  standard: MPP (Tempo rail) — declared in each spec's x-mpp extension
  type: payment
- description: 'Not a client credential: every response from hivetrust, hivegate and hivebank carries an issuer DID (did:hive:hivetrust, did:hive:hivegate, did:hive:hivebank), a timestamp, a base64url Ed25519 signature and a pointer to the public key at /v1/prov/pubkey ("every door 200s, every byte signed"). Observed on 2026-09-19 on GET / and POST /mcp responses.'
  headers:
  - X-Hive-Prov-Iss
  - X-Hive-Prov-Ts
  - X-Hive-Prov-Sig
  - X-Hive-Prov-Pubkey
  - X-Hive-Prov-Payload
  name: HiveProvenanceHeaders
  pubkeys:
  - algorithm: Ed25519
    issuer: did:hive:hivetrust
    url: https://hivetrust.hiveagentiq.com/v1/prov/pubkey
  - algorithm: Ed25519
    issuer: did:hive:hivegate
    url: https://hivegate.hiveagentiq.com/v1/prov/pubkey
  standard: Ed25519 over a canonical request line ("smash.prov")
  type: response-signature
slug: hiveagentiq-com-authentication
source_filename: hiveagentiq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://hivetrust.hiveagentiq.com/.well-known/hivetrust.json\nderived_from:\n- openapi/hiveagentiq-com-hivetrust-openapi.json\n- openapi/hiveagentiq-com-hivegate-openapi.json\n- openapi/hiveagentiq-com-hivebank-openapi.json\n- openapi/hiveagentiq-com-hivelaw-openapi.json\ndocs:\n- https://hivegate.hiveagentiq.com/llms.txt\n- https://hivegate.hiveagentiq.com/.well-known/hivegate.json\n- https://hivetrust.hiveagentiq.com/.well-known/mcp.json\n- https://github.com/srotzin/hivetrust#api-reference\n- https://thehiveryiq.com/onboard.html\nsummary:\n  types: [apiKey, http-bearer, payment, signature]\n  api_key_in: [header]\n  oauth2_flows: []\n  bearer: true\n  credential_classes: 5\n  headline: >-\n    None of the four OpenAPI documents declares a securityScheme (derive-authentication.py found nothing to derive), so\n    this profile is assembled from the discovery documents, llms.txt files, the MCP initialize instructions, the source\n\
  \    READMEs and the live 401/402 envelopes. The identity credential is a Hive DID (did:hive:*) issued free by POST\n    https://hivegate.hiveagentiq.com/v1/gate/onboard (\"first DID is free, no payment required\"), presented either as an\n    X-API-Key (ht_-prefixed per the README), as Authorization: Bearer did:hive:*, or as an X-Hive-DID header; HiveGate\n    guest sessions use Bearer hgate_* access tokens. Beyond identity, most operations are metered: an unauthenticated or\n    unpaid call gets an HTTP 402 with the USDC amount and rails, settled through x402 (USDC/USDT on Base) or the MPP\n    (Tempo) rail declared in every spec's x-mpp block. No OAuth 2.0, no OIDC, no RFC 9728 metadata on any host.\nschemes:\n- name: HiveDIDApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    \"Authentication via X-API-Key header\" (hivetrust README); examples use ht_your_api_key. The key is issued with the\n    DID at onboarding (\"returns a did:hive:* identifier +\
  \ API key\" — thehiveryiq.com/onboard.html; \"DID issuance, API key\n    provisioning\" — HiveGate ai-plugin.json). The MCP manifest states \"tools_list: public, tools_call: X-API-Key or\n    Authorization: Bearer did:hive:* required\".\n  issuance:\n    operation: POST https://hivegate.hiveagentiq.com/v1/gate/onboard\n    cost: free for the first DID; premium sovereign DID $4.99 (llms.txt) or $9.99 (402 envelope)\n    signup: agent_name + email in the request body (402 envelope quick_start)\n  sources:\n  - https://github.com/srotzin/hivetrust#api-reference\n  - https://hivetrust.hiveagentiq.com/.well-known/mcp.json\n  - https://hivegate.hiveagentiq.com/.well-known/hivegate.json\n- name: HiveDIDBearer\n  type: http\n  scheme: bearer\n  bearer_format: did:hive:* (agent DID) or hgate_* (HiveGate guest access token)\n  description: >-\n    hivegate.json authentication.methods lists \"Authorization: Bearer did:hive:*\" and \"Authorization: Bearer hgate_*\";\n    the HiveTrust MCP server's\
  \ initialize instructions say tools/call for write operations requires \"a registered Hive\n    DID via X-API-Key or Authorization: Bearer did:hive:* header\". The hgate_ token is returned by hivegate_register_guest\n    / POST /v1/gate/register-guest and is required by hivegate_execute (access_token, \"Guest access token (hgate_*)\").\n  sources:\n  - https://hivegate.hiveagentiq.com/.well-known/hivegate.json\n  - mcp/hiveagentiq-com-hivegate-mcp-tools.json\n- name: HiveDIDHeader\n  type: apiKey\n  in: header\n  parameter: X-Hive-DID\n  aliases: [x-hive-did, x-did, X-HiveTrust-DID]\n  description: >-\n    The \"sovereign handshake\": \"present X-Hive-DID header on non-free endpoints\" (HiveGate llms.txt); the 402 envelope\n    lists headers_required [\"X-Hive-DID\"] and says \"After checkout, include your issued did:hive: in the X-Hive-DID\n    header on every request\". hivegate.json also names x-did and X-HiveTrust-DID. The same header claims the\n    first-call-free offer (\"New here?\
  \ Add header 'x-hive-did' to claim your first call free\" — agent card bogo block).\n  sources:\n  - https://hivegate.hiveagentiq.com/llms.txt\n  - a2a/hiveagentiq-com-agent-card.json\n- name: x402Payment\n  type: payment\n  standard: x402 (HTTP 402)\n  in: header\n  parameter: X-Payment\n  description: >-\n    Every paid route answers 402. Observed on HiveGate: {\"error\":\"payment_required\",\"code\":\"HIVE_402\", \"detail\":{\"x402\":\n    {\"version\":\"1.0\",\"amount_usdc\":9.99,\"payment_methods\":[\"stripe-checkout\",\"x402-usdc\",\"x402-aleo\"],\"headers_required\":\n    [\"X-Hive-DID\"]}}}. The HiveGate hive-payments.json names the header: \"x402\": {\"supported\": true, \"header\": \"X-Payment\",\n    \"currency\": \"USDC\", \"network\": \"base\"}. llms.txt: \"Paid surfaces return a 402 with amount_min_usd — the floor price.\n    Submit any value >= that floor.\" Settlement rails: USDC/USDT on Base to treasury 0x15184Bf50B3d3F52b60434f8942b7D52F2eB436E,\n    USDC on Solana, USDCx/USAD/ALEO\
  \ on Aleo. The hivetrust ai-plugin.json declares auth.type \"none\" with a payment block —\n    payment, not a credential, is the gate.\n  observed:\n  - {url: 'https://hivegate.hiveagentiq.com/v1/gate/adapters', http_status: 402, code: HIVE_402}\n  - {url: 'https://hivegate.hiveagentiq.com/docs', http_status: 402, code: HIVE_402}\n  sources:\n  - well-known/hiveagentiq-com-hivegate-hive-payments.json\n  - https://hivegate.hiveagentiq.com/llms.txt\n- name: MPPPayment\n  type: payment\n  standard: MPP (Tempo rail) — declared in each spec's x-mpp extension\n  description: >-\n    All four OpenAPIs carry x-mpp: {realm, payment: {method: tempo, currency: 0x20c0…b50, decimals: 6, recipient}, rails:\n    [x402, mpp]} and per-operation x-mpp-charge {amount, intent: charge} in 6-decimal USDC units ($0.10 = \"100000\").\n    No MPP challenge was observed live; recorded from the contract only.\n  sources:\n  - openapi/hiveagentiq-com-hivetrust-openapi.json\n- name: HiveProvenanceHeaders\n  type:\
  \ response-signature\n  standard: Ed25519 over a canonical request line (\"smash.prov\")\n  headers: [X-Hive-Prov-Iss, X-Hive-Prov-Ts, X-Hive-Prov-Sig, X-Hive-Prov-Pubkey, X-Hive-Prov-Payload]\n  description: >-\n    Not a client credential: every response from hivetrust, hivegate and hivebank carries an issuer DID (did:hive:hivetrust,\n    did:hive:hivegate, did:hive:hivebank), a timestamp, a base64url Ed25519 signature and a pointer to the public key at\n    /v1/prov/pubkey (\"every door 200s, every byte signed\"). Observed on 2026-09-19 on GET / and POST /mcp responses.\n  pubkeys:\n  - {issuer: 'did:hive:hivetrust', url: 'https://hivetrust.hiveagentiq.com/v1/prov/pubkey', algorithm: Ed25519}\n  - {issuer: 'did:hive:hivegate', url: 'https://hivegate.hiveagentiq.com/v1/prov/pubkey', algorithm: Ed25519}\nunauthenticated_envelope:\n  hivetrust_and_hivebank:\n    http_status: 401\n    body: '{\"status\":\"unregistered_agent\",\"error\":\"agent_not_registered\",\"message\":\"Welcome to Hive\
  \ Civilization — register your agent DID to unlock 21 services across 12 layers.\",\"onboard\":{\"url\":\"https://hivegate.hiveagentiq.com/v1/gate/onboard\", ...}, \"recruitment\": {...}}'\n    observed_on: ['GET /v1/agents', 'GET /v1/webhooks', 'GET /v1/bond/tiers', 'GET /v1/bond/pool', 'GET /v1/liquidation/stats', 'GET /v1/reputation/status/{did}', 'GET /v1/bank/stats']\n  hivegate:\n    http_status: 402\n    body: '{\"error\":\"payment_required\",\"code\":\"HIVE_402\", ...}'\n    observed_on: ['GET /v1/gate/adapters', 'GET /v1/gate/stats', 'GET /v1/gate/directory', 'GET /v1/mcp/tools', 'GET /docs']\npublic_operations:\n  note: >-\n    Free without any credential, observed 200 on 2026-09-19: hivetrust GET /health, /v1/stats, /v1/pricing/status,\n    /v1/oracle/streams, /v1/trust/lookup/{did}, /v1/prov/pubkey, /openapi.json, /llms.txt, /.well-known/*; hivegate\n    GET /health, /v1/gate/queue/stats, /v1/gate/sample, /openapi.json, /llms.txt, /.well-known/*; hivelaw GET /health,\n    /v1/jurisdictions,\
  \ /v1/case-law/stats, /v1/mcp/tools; hivebank GET /health, /openapi.json, /llms.txt. MCP initialize\n    and tools/list answer anonymously on hivetrust, hivegate and hivebank.\ndiscovery:\n  oauth_authorization_server: 'hivetrust 200 but a catch-all JSON \"not a real endpoint\" body; hivegate 404; hivelaw 404; hivebank 200 catch-all hint body'\n  oauth_protected_resource: same pattern — no RFC 9728 metadata on any host\n  openid_configuration: same pattern — no OIDC\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiveagentiq-com/refs/heads/main/authentication/hiveagentiq-com-authentication.yml
summary_line: apiKey/http-bearer/payment/signature · 6 schemes
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Decentralized Identity
- Verifiable Credentials
- Trust Scoring
- Stablecoins
- Insurance
- Compliance
- Agent-Native
- United States
---
