---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: thehiveryiq-com-hivemorph-openapi.yml
  format: yaml
  label: Hive Receipts and Agent Commerce API (HiveMorph)
  slug: hivemorph-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thehiveryiq-com/refs/heads/main/openapi/thehiveryiq-com-hivemorph-openapi.yml
- filename: thehiveryiq-com-hivecompute-openapi.yml
  format: yaml
  label: HiveCompute Inference Router API
  slug: hivecompute-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thehiveryiq-com/refs/heads/main/openapi/thehiveryiq-com-hivecompute-openapi.yml
auth_types:
- none
- x402-payment
- apiKey
- ed25519-signed-request
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Thehiveryiq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hive Civilization secures its APIs with none, x402-payment, apiKey, and ed25519-signed-request across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hive Civilization
provider_slug: thehiveryiq-com
scheme_count: 6
schemes:
- applies_to: Discovery documents (/.well-known/*, /openapi.json, /llms.txt, /pricing, /status, /manifest, /a2a GET), the free tier (POST /v1/receipt/free), receipt verification (POST /v1/receipt/verify, GET /v1/receipt/{receipt_id}), x402 quotes (POST /v1/x402/quote), GET /v1/settlement/reference, GET /v1/hktn/lookup, POST /v1/delegation/check, POST /v1/delegation/revoke/{jti}, MCP initialize/tools/list on both MCP hosts, HiveCompute POST /v1/compute/estimate and GET /v1/compute/models
  evidence: 'Observed live 2026-09-19: POST /v1/receipt/free -> 201 with no credential; POST /v1/x402/quote {} -> 200; POST /v1/compute/estimate -> 200; tools/list -> 200 on api.thehiveryiq.com/mcp and hive-mcp-gateway.onrender.com/mcp. The /agents page: "Verify and quote are always free", "No API key, no signup".'
  name: none
  sources:
  - openapi/thehiveryiq-com-hivemorph-openapi.yml
  - openapi/thehiveryiq-com-hivecompute-openapi.yml
  type: none
- applies_to: Every metered operation (receipt emit, rubric select, prospector score, rosetta normalize after the first 25 free calls per agent, compute.chat, most gateway MCP tools)
  challenge:
    hivecompute_host:
      headers:
        payment-required: '<base64url JSON: {"x402Version":1,"accepts":[{"scheme":"exact","network":"base","maxAmountRequired":"20000","resource":"https://api.thehiveryiq.com/v1/compute/chat/completions","payTo":"0x15184Bf5...436E","maxTimeoutSeconds":300,"asset":"0x833589fC...02913","extra":{"name":"USD Coin","version":"2","assetTransferMethod":"eip3009"}}]}>'
        www-authenticate: x402
      note: 'The two hosts speak two different x402 envelope generations (x402_version 0.1 JSON body vs x402Version 1 base64 PAYMENT-REQUIRED header + www-authenticate: x402).'
      observed: POST /v1/compute/chat/completions without payment, 2026-09-19
    receipts_host:
      body: '{"error":"payment_required","message":"This endpoint requires a micropayment via the x402 protocol. Submit payment proof via X-Payment header or POST /v1/x402/proof/submit.","payment":{"x402_version":"0.1","nonce":"<uuid>","resource":"/v1/receipt/emit","amount_usd":0.0008,"payment_endpoint":"/v1/x402/proof/submit","expires_at":<unix>,"accepts":[{"chain":"base","asset":"USDC","scheme":"exact","recipient":"0x15184bf5...436e","asset_contract":"0x833589fC...02913","decimals":6,"amount_atomic":"800"}, ...USDT/base, USDC+USDT/solana, USDT/ethereum]}}'
      headers:
        x-payment-required: 'true'
      observed: POST /v1/receipt/emit without payment, 2026-09-19
    status: 402
  name: x402
  protocol: x402
  settlement:
    client_sdk: hive-rosetta (npm/PyPI 0.1.0) implements the 402 -> sign -> retry loop
    header_alternative: X-Payment header carrying the proof
    rails: 'https://receipts.thehiveryiq.com/v1/x402/rails and /.well-known/x402.json: USDC + USDT on Base (8453), USDC + USDT on Solana, USDT on Ethereum; scheme exact; EIP-3009 transferWithAuthorization on Base'
    submit: 'POST /v1/x402/proof/submit (operationId submit_proof_v1_x402_proof_submit_post): "Submit a payment proof for a pending 402 nonce. On success, returns an access token (5-minute TTL) that can be used in the X-Hive-Access header to bypass 402 for the same path."'
  sources:
  - openapi/thehiveryiq-com-hivemorph-openapi.yml
  - openapi/thehiveryiq-com-hivecompute-openapi.yml
  - https://receipts.thehiveryiq.com/.well-known/x402.json
  type: payment-challenge
- applies_to: Short-lived (5-minute) access token minted by /v1/x402/proof/submit for the paid path; also a header parameter on POST /v1/activation/keys
  in: header
  name: X-Hive-Access
  parameter: X-Hive-Access
  sources:
  - openapi/thehiveryiq-com-hivemorph-openapi.yml
  type: apiKey
- applies_to: 'Tenant / portal surface: POST /tenants/:id/receipts (documented on /developers as the "authenticated tenant route"), GET /tenants/:id/evidence, wallet (/v1/wallet/register, /v1/wallet/me), designer mint, bounty admin; the pricing page lists "API key auth via Bearer header" on the Builder tier'
  evidence: 'POST /v1/portal/{tenant_id}/api-key/revoke description: ''Pass { "key": "tk_live_..." } to revoke a specific key; omit to revoke all.'' The ''authorization'' header parameter is declared on 8 operations.'
  issuance: Tenant onboarding wizard at https://thehiveryiq.com/onboard/ ; keys revocable via portal_revoke_key_v1_portal__tenant_id__api_key_revoke_post
  key_prefix: tk_live_
  name: tenant API key (Bearer)
  scheme: bearer
  sources:
  - openapi/thehiveryiq-com-hivemorph-openapi.yml
  - https://thehiveryiq.com/pricing/
  type: http
- applies_to: 'Operator-only operations (x402 pricing/rails admin, evaluator start/stop, perp liquidation, dashboards, site-traffic redaction): 34 header parameters across ~20 operations'
  in: header
  name: X-Admin-Api-Key / x-admin-token / X-Hive-Trust
  note: Not customer credentials; recorded so an agent does not mistake these operations for callable surface.
  parameters:
  - X-Admin-Api-Key
  - x-admin-token
  - X-Hive-Trust
  sources:
  - openapi/thehiveryiq-com-hivemorph-openapi.yml
  type: apiKey
- algorithm: Ed25519
  applies_to: 'POST /v1/mos/intel/register: "site-did + x-hive-nonce + x-hive-sig (ed25519)" per its description; agent identity elsewhere is carried as agent_did (did:hive:...) in request bodies without signature'
  headers:
  - x-hive-nonce
  - x-hive-sig
  name: DID-signed request
  sources:
  - openapi/thehiveryiq-com-hivemorph-openapi.yml
  type: signature
slug: thehiveryiq-com-authentication
source_filename: thehiveryiq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://thehiveryiq.com/agents\nderived_from:\n- openapi/thehiveryiq-com-hivemorph-openapi.yml\n- openapi/thehiveryiq-com-hivecompute-openapi.yml\ndocs:\n- https://thehiveryiq.com/agents\n- https://thehiveryiq.com/developers\n- https://thehiveryiq.com/pricing/\n- https://receipts.thehiveryiq.com/llms.txt\n- https://receipts.thehiveryiq.com/.well-known/x402.json\nsummary:\n  types:\n  - none\n  - x402-payment\n  - apiKey\n  - ed25519-signed-request\n  api_key_in:\n  - header\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  note: 'NEITHER OpenAPI declares a securitySchemes block and 0 of 937 HiveMorph operations carry a security[] requirement,\n    so derive-authentication.py has nothing to read: the entire auth model lives in operation descriptions, header\n    parameters and the docs. Reconstructed from those. The dominant model is ''no credential, pay per call'': discovery\n    and the free tier need nothing,\
  \ and paid operations answer HTTP 402 with an x402 payment challenge instead of\n    401. Tenant API keys (Bearer) exist for the tenant/portal surface; operator-only admin headers appear on a few\n    dozen internal operations.'\nschemes:\n- name: none\n  type: none\n  applies_to: Discovery documents (/.well-known/*, /openapi.json, /llms.txt, /pricing, /status, /manifest, /a2a\n    GET), the free tier (POST /v1/receipt/free), receipt verification (POST /v1/receipt/verify, GET /v1/receipt/{receipt_id}),\n    x402 quotes (POST /v1/x402/quote), GET /v1/settlement/reference, GET /v1/hktn/lookup, POST /v1/delegation/check,\n    POST /v1/delegation/revoke/{jti}, MCP initialize/tools/list on both MCP hosts, HiveCompute POST /v1/compute/estimate\n    and GET /v1/compute/models\n  evidence: 'Observed live 2026-09-19: POST /v1/receipt/free -> 201 with no credential; POST /v1/x402/quote {} ->\n    200; POST /v1/compute/estimate -> 200; tools/list -> 200 on api.thehiveryiq.com/mcp and hive-mcp-gateway.onrender.com/mcp.\n\
  \    The /agents page: \"Verify and quote are always free\", \"No API key, no signup\".'\n  sources:\n  - openapi/thehiveryiq-com-hivemorph-openapi.yml\n  - openapi/thehiveryiq-com-hivecompute-openapi.yml\n- name: x402\n  type: payment-challenge\n  protocol: x402\n  applies_to: Every metered operation (receipt emit, rubric select, prospector score, rosetta normalize after the\n    first 25 free calls per agent, compute.chat, most gateway MCP tools)\n  challenge:\n    status: 402\n    receipts_host:\n      headers:\n        x-payment-required: 'true'\n      body: '{\"error\":\"payment_required\",\"message\":\"This endpoint requires a micropayment via the x402 protocol.\n        Submit payment proof via X-Payment header or POST /v1/x402/proof/submit.\",\"payment\":{\"x402_version\":\"0.1\",\"nonce\":\"<uuid>\",\"resource\":\"/v1/receipt/emit\",\"amount_usd\":0.0008,\"payment_endpoint\":\"/v1/x402/proof/submit\",\"expires_at\":<unix>,\"accepts\":[{\"chain\":\"base\",\"asset\":\"USDC\",\"\
  scheme\":\"exact\",\"recipient\":\"0x15184bf5...436e\",\"asset_contract\":\"0x833589fC...02913\",\"decimals\":6,\"amount_atomic\":\"800\"},\n        ...USDT/base, USDC+USDT/solana, USDT/ethereum]}}'\n      observed: POST /v1/receipt/emit without payment, 2026-09-19\n    hivecompute_host:\n      headers:\n        www-authenticate: x402\n        payment-required: '<base64url JSON: {\"x402Version\":1,\"accepts\":[{\"scheme\":\"exact\",\"network\":\"base\",\"maxAmountRequired\":\"20000\",\"resource\":\"https://api.thehiveryiq.com/v1/compute/chat/completions\",\"payTo\":\"0x15184Bf5...436E\",\"maxTimeoutSeconds\":300,\"asset\":\"0x833589fC...02913\",\"extra\":{\"name\":\"USD\n          Coin\",\"version\":\"2\",\"assetTransferMethod\":\"eip3009\"}}]}>'\n      observed: POST /v1/compute/chat/completions without payment, 2026-09-19\n      note: 'The two hosts speak two different x402 envelope generations (x402_version 0.1 JSON body vs x402Version\n        1 base64 PAYMENT-REQUIRED header + www-authenticate:\
  \ x402).'\n  settlement:\n    submit: 'POST /v1/x402/proof/submit (operationId submit_proof_v1_x402_proof_submit_post): \"Submit a payment\n      proof for a pending 402 nonce. On success, returns an access token (5-minute TTL) that can be used in the\n      X-Hive-Access header to bypass 402 for the same path.\"'\n    header_alternative: X-Payment header carrying the proof\n    rails: 'https://receipts.thehiveryiq.com/v1/x402/rails and /.well-known/x402.json: USDC + USDT on Base (8453),\n      USDC + USDT on Solana, USDT on Ethereum; scheme exact; EIP-3009 transferWithAuthorization on Base'\n    client_sdk: hive-rosetta (npm/PyPI 0.1.0) implements the 402 -> sign -> retry loop\n  sources:\n  - openapi/thehiveryiq-com-hivemorph-openapi.yml\n  - openapi/thehiveryiq-com-hivecompute-openapi.yml\n  - https://receipts.thehiveryiq.com/.well-known/x402.json\n- name: X-Hive-Access\n  type: apiKey\n  in: header\n  parameter: X-Hive-Access\n  applies_to: Short-lived (5-minute) access token minted\
  \ by /v1/x402/proof/submit for the paid path; also a header\n    parameter on POST /v1/activation/keys\n  sources:\n  - openapi/thehiveryiq-com-hivemorph-openapi.yml\n- name: tenant API key (Bearer)\n  type: http\n  scheme: bearer\n  key_prefix: tk_live_\n  applies_to: 'Tenant / portal surface: POST /tenants/:id/receipts (documented on /developers as the \"authenticated\n    tenant route\"), GET /tenants/:id/evidence, wallet (/v1/wallet/register, /v1/wallet/me), designer mint, bounty\n    admin; the pricing page lists \"API key auth via Bearer header\" on the Builder tier'\n  evidence: 'POST /v1/portal/{tenant_id}/api-key/revoke description: ''Pass { \"key\": \"tk_live_...\" } to revoke a\n    specific key; omit to revoke all.'' The ''authorization'' header parameter is declared on 8 operations.'\n  issuance: Tenant onboarding wizard at https://thehiveryiq.com/onboard/ ; keys revocable via portal_revoke_key_v1_portal__tenant_id__api_key_revoke_post\n  sources:\n  - openapi/thehiveryiq-com-hivemorph-openapi.yml\n\
  \  - https://thehiveryiq.com/pricing/\n- name: X-Admin-Api-Key / x-admin-token / X-Hive-Trust\n  type: apiKey\n  in: header\n  parameters:\n  - X-Admin-Api-Key\n  - x-admin-token\n  - X-Hive-Trust\n  applies_to: 'Operator-only operations (x402 pricing/rails admin, evaluator start/stop, perp liquidation, dashboards,\n    site-traffic redaction): 34 header parameters across ~20 operations'\n  note: Not customer credentials; recorded so an agent does not mistake these operations for callable surface.\n  sources:\n  - openapi/thehiveryiq-com-hivemorph-openapi.yml\n- name: DID-signed request\n  type: signature\n  headers:\n  - x-hive-nonce\n  - x-hive-sig\n  algorithm: Ed25519\n  applies_to: 'POST /v1/mos/intel/register: \"site-did + x-hive-nonce + x-hive-sig (ed25519)\" per its description;\n    agent identity elsewhere is carried as agent_did (did:hive:...) in request bodies without signature'\n  sources:\n  - openapi/thehiveryiq-com-hivemorph-openapi.yml\nresponse_provenance:\n  note: 'Authentication\
  \ of the SERVER to the client is a first-class feature: api.thehiveryiq.com signs every response\n    (X-Hive-Prov-Iss did:hive:hivecompute, X-Hive-Prov-Ts, X-Hive-Prov-Sig, X-Hive-Prov-Pubkey -> /v1/prov/pubkey,\n    X-Hive-Prov-Payload) and publishes a JWKS; receipts.thehiveryiq.com publishes its Ed25519 verifier key at /v1/prov/pubkey\n    and /trust.json (issuer did:hive:hivemorph, epoch 1, rotation \"on-incident or annual\"); passport.thehiveryiq.com\n    does the same for did:hive:hive-passport.'\n  observed: Response headers on GET https://api.thehiveryiq.com/openapi.json, 2026-09-19\ngaps:\n- No securitySchemes in either OpenAPI, so generated clients cannot attach credentials or model the 402 flow.\n- No OAuth 2.0 / OIDC anywhere (RFC 8414 / 9728 / OIDC discovery all absent on every host, including both MCP hosts).\n- 'Key lifecycle: no documented rotation for tenant keys; the security page states \"no verified 90-day automatic\n  invalidation policy\".'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thehiveryiq-com/refs/heads/main/authentication/thehiveryiq-com-authentication.yml
summary_line: none/x402-payment/apiKey/ed25519-signed-request · 6 schemes
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Receipts
- Digital Signature
- Post-Quantum Cryptography
- Attestation
- Decentralized Identity
- Stablecoins
- Inference
- LLM Routing
- Compliance
- agent-native
- United States
---
