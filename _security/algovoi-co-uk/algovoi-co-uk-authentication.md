---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: algovoi-co-uk-pay-openapi.yml
  format: yaml
  label: AlgoVoi Pay (Payable Core) API
  slug: algovoi-pay-payable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-pay-openapi.yml
- filename: algovoi-co-uk-gateway-openapi.yml
  format: yaml
  label: AlgoVoi Gateway API
  slug: algovoi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-gateway-openapi.yml
- filename: algovoi-co-uk-clinic-openapi.yml
  format: yaml
  label: AlgoVoi RFC 9421 Clinic (Verifiable-Comms Agent) API
  slug: algovoi-rfc9421-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-clinic-openapi.yml
- filename: algovoi-co-uk-agent-trust-bench-openapi.yml
  format: yaml
  label: AlgoVoi Agent Trust Bench API
  slug: algovoi-agent-trust-bench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-agent-trust-bench-openapi.yml
- filename: algovoi-co-uk-audit-verifier-openapi.yml
  format: yaml
  label: AlgoVoi Audit Verifier API
  slug: algovoi-audit-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-audit-verifier-openapi.yml
- filename: algovoi-co-uk-gateway-openapi.yml
  format: yaml
  label: AlgoVoi MCP Server
  slug: algovoi-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-gateway-openapi.yml
auth_types:
- http-bearer
- apiKey(header)
- payment-as-auth(x402)
- payment-as-auth(mpp)
- hmac-webhook-signature
- session-token
- none
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Algovoi Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlgoVoi secures its APIs with http-bearer, apiKey(header), payment-as-auth(x402), payment-as-auth(mpp), hmac-webhook-signature, session-token, and none across 9 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AlgoVoi
provider_slug: algovoi-co-uk
scheme_count: 9
schemes:
- applies_to: api.algovoi.co.uk (canonical) and the cloud.algovoi.co.uk proxy; the stdio MCP server and every framework adapter carry the same key
  companion_header: X-Tenant-Id
  description: '"Authorization: Bearer <YOUR_API_KEY>" plus "X-Tenant-Id: <YOUR_TENANT_ID>" on every authenticated request; the key proves you may act, the tenant header selects which tenant. Keys are shown once at creation and stored one-way hashed. Keys are bound to a mode — test-mode keys reach testnet networks only, live-mode keys reach mainnet only after KYC — and cannot switch modes. Rotation: one click, old and new keys both valid for 30 days, then the old key is revoked.'
  docs: https://docs.algovoi.co.uk/api-reference/authentication
  errors:
    401: invalid_api_key
    403: tenant_id_mismatch / missing scope
    422: kyb_required_for_mainnet
  header: Authorization
  id: tenant-api-key
  key_prefix: algv_
  observed: POST /v1/verify and GET /v1/customers without credentials → 401 {"detail":"Unauthorized"}; /a2a/jsonrpc and /extendedAgentCard likewise 401
  obtain: https://dash.algovoi.co.uk (Settings → API keys); trial accounts via https://dash.algovoi.co.uk/signup or https://api.algovoi.co.uk/signup
  scheme: bearer
  type: http
- applies_to: operator / control-plane endpoints
  description: Admin keys carry a scope list; "most tenant integrations don't need admin keys at all". Two MCP tools (list_mpp_subscriptions, cancel_mpp_subscription) require an admin-scope key. Not OAuth scopes — no OAuthScopes artifact is emitted.
  header: Authorization
  id: admin-control-plane-key
  key_prefix: algvc_
  scheme: bearer
  scopes:
  - tenants:admin
  - apikeys:admin
  - kyb:write
  - live:activate
  - payments:read
  - audit:read
  type: http
- applies_to: POST /auth/token (exchange_atb_cert_auth_token_post) and GET /auth/token/status (session_status_auth_token_status_get)
  description: 'An agent exchanges an ATB ZKP certificate (X-ATB-ZK-Credential) or a federation token for a spend-capped session token, using normal API-key auth for that one request; the returned token is then presented as "Authorization: Bearer <token>" without X-Tenant-Id (tenant id is read from the token claims). 401 when invalid or expired.'
  docs: https://docs.algovoi.co.uk/agent-session-auth
  header: Authorization
  id: agent-session-token
  scheme: bearer
  type: http
- applies_to: POST /mandate/pay (mandate_pay_mandate_pay_post)
  description: A mandate JWT is passed as a standard HTTP Bearer token; no X-Tenant-Id — mandate tokens are cross-tenant.
  header: Authorization
  id: mandate-jwt
  scheme: bearer
  type: http
- applies_to: pay.algovoi.co.uk /pay/v1/* (payment is the only credential), api.algovoi.co.uk /mpp/probe, /mpp/{resource_id}, /protected/{resource_id}, /r/{tenant}/{resource}, and mcp.algovoi.co.uk/mcp tool calls
  challenge: HTTP 402 with a JSON accepts[] body and a base64 payment-required header; on the pay rail every 402 carries one accept per enabled lane with payTo, amount (10000 micro-USDC) and a 1800-second payment_reference challenge token
  description: '"No API key/bearer. Each paid skill returns an x402 v2 402 challenge ... pay the USDC amount to payTo on your chosen lane, bound per that lane''s scheme, then resubmit with the X-PAYMENT proof." Mined-tx lanes (Algorand, Voi, Stellar, Hedera, Solana, Tempo) weld the challenge into the tx note/memo/reference; EVM EIP-3009 lanes (Base, Monad, Polygon, Arbitrum, OP, Arc) accept a stock signed TransferWithAuthorization with an optional nonce weld. A2A over the same rail uses the a2a-x402 extension (payment-required task state).'
  docs: https://docs.algovoi.co.uk/algovoi-pay
  header: X-PAYMENT
  id: x402-payment
  observed: GET https://pay.algovoi.co.uk/pay/v1/verify/receipt → 402, 13,977-byte accepts[] body, payment-required header; POST tools/list on mcp.algovoi.co.uk/mcp → 402 x402 v1 challenge
  protocol: x402 (v2 on pay.algovoi.co.uk; v1 and v2 on api.algovoi.co.uk)
  type: payment
- applies_to: api.algovoi.co.uk /mpp/* and /mpp/sub/*
  header: 'WWW-Authenticate: Payment (challenge) / PAYMENT-SIGNATURE (proof, declared as a header parameter in the gateway spec)'
  id: mpp-payment
  observed: 'GET https://api.algovoi.co.uk/mpp/probe → 402 with WWW-Authenticate: Payment realm="api.algovoi.co.uk", id="algovoi-mpp-probe-static-v1", method="tempo", intent="charge", expires=..., request=<base64>'
  protocol: MPP (Machine Payments Protocol) — HTTP "Payment" authentication scheme
  type: payment
- algorithm: HMAC-SHA256 over "{t}.{raw_body}"; header format t={unix_ts},v1={hex}; ±300 s tolerance; constant-time compare; 30-day dual-secret rotation window
  direction: inbound to the tenant (AlgoVoi signs outbound webhooks)
  docs: https://docs.algovoi.co.uk/integrations/outbound-webhooks
  header: X-AlgoVoi-Signature
  id: webhook-signature
  key_prefix: algvw_
  type: hmac
- applies_to: Optional on payment-gated gateway operations (declared as header parameters); presenting a valid Falcon-1024 or Bulletproofs ATB Pass Certificate earns a 20% discount on the challenge amount
  docs: https://docs.algovoi.co.uk/atb-reputation-credential
  id: reputation-credentials
  in: header
  name: X-ATB-Credential / X-ATB-ZK-Credential
  type: apiKey
- applies_to: agents.algovoi.co.uk (clinic REST, A2A and MCP), verify.algovoi.co.uk (audit verifier), agent-trust-bench.algovoi.co.uk (/freebie, /discovery/resources, /stats.json; profiles answer 402), pay.algovoi.co.uk free tiers (/v1/receipt/verify 120/min, /verify/rfc9421 60/min), api.algovoi.co.uk /health, /compliance/attestation, /discovery/resources, /.well-known/*
  description: Public, no credential; abuse control is per-IP rate limiting.
  id: anonymous
  type: none
slug: algovoi-co-uk-authentication
source_filename: algovoi-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://docs.algovoi.co.uk/api-reference/authentication\ndocs: https://docs.algovoi.co.uk/api-reference/authentication\nspec: [openapi/algovoi-co-uk-gateway-openapi.yml, openapi/algovoi-co-uk-pay-openapi.yml, openapi/algovoi-co-uk-clinic-openapi.yml, openapi/algovoi-co-uk-agent-trust-bench-openapi.yml, openapi/algovoi-co-uk-audit-verifier-openapi.yml]\nsummary:\n  types: [http-bearer, apiKey(header), payment-as-auth(x402), payment-as-auth(mpp), hmac-webhook-signature, session-token, none]\n  api_key_in: [header]\n  oauth2_flows: []\n  transport: HTTPS only (TLS 1.3 at the Cloudflare edge, HSTS preload on every host probed)\n  note: >-\n    NONE of the five OpenAPIs declares components.securitySchemes or operation-level security — the gateway spec\n    instead declares `authorization` and `x-tenant-id` as plain header parameters on 53 / 48 operations, and the\n    pay spec declares `x-payment` as an optional header on paid operations.\
  \ The authentication model therefore comes\n    from the docs and from live probes, not the contracts; overlays/ adds the schemes as an enhancement. Four\n    surfaces, four models: the tenant gateway is a static Bearer key plus a tenant selector; the pay rail has no\n    credential at all (the on-chain payment presented in X-PAYMENT is the authorization); the clinic, the audit\n    verifier and the Agent Trust Bench are anonymous; and the ulu MCP server gates tool calls with an x402 402.\n    There is no OAuth 2.0, no OIDC and no dynamic client registration anywhere in the estate (every\n    /.well-known/openid-configuration and oauth-* probe is 404/405).\nschemes:\n- id: tenant-api-key\n  type: http\n  scheme: bearer\n  header: Authorization\n  companion_header: X-Tenant-Id\n  key_prefix: algv_\n  applies_to: api.algovoi.co.uk (canonical) and the cloud.algovoi.co.uk proxy; the stdio MCP server and every framework adapter carry the same key\n  description: >-\n    \"Authorization: Bearer\
  \ <YOUR_API_KEY>\" plus \"X-Tenant-Id: <YOUR_TENANT_ID>\" on every authenticated request; the\n    key proves you may act, the tenant header selects which tenant. Keys are shown once at creation and stored\n    one-way hashed. Keys are bound to a mode — test-mode keys reach testnet networks only, live-mode keys reach\n    mainnet only after KYC — and cannot switch modes. Rotation: one click, old and new keys both valid for 30 days,\n    then the old key is revoked.\n  obtain: https://dash.algovoi.co.uk (Settings → API keys); trial accounts via https://dash.algovoi.co.uk/signup or https://api.algovoi.co.uk/signup\n  observed: 'POST /v1/verify and GET /v1/customers without credentials → 401 {\"detail\":\"Unauthorized\"}; /a2a/jsonrpc and /extendedAgentCard likewise 401'\n  errors: {401: invalid_api_key, 403: tenant_id_mismatch / missing scope, 422: kyb_required_for_mainnet}\n  docs: https://docs.algovoi.co.uk/api-reference/authentication\n- id: admin-control-plane-key\n  type: http\n  scheme:\
  \ bearer\n  header: Authorization\n  key_prefix: algvc_\n  applies_to: operator / control-plane endpoints\n  scopes: [tenants:admin, apikeys:admin, kyb:write, live:activate, payments:read, audit:read]\n  description: Admin keys carry a scope list; \"most tenant integrations don't need admin keys at all\". Two MCP tools (list_mpp_subscriptions, cancel_mpp_subscription) require an admin-scope key. Not OAuth scopes — no OAuthScopes artifact is emitted.\n- id: agent-session-token\n  type: http\n  scheme: bearer\n  header: Authorization\n  applies_to: 'POST /auth/token (exchange_atb_cert_auth_token_post) and GET /auth/token/status (session_status_auth_token_status_get)'\n  description: >-\n    An agent exchanges an ATB ZKP certificate (X-ATB-ZK-Credential) or a federation token for a spend-capped\n    session token, using normal API-key auth for that one request; the returned token is then presented as\n    \"Authorization: Bearer <token>\" without X-Tenant-Id (tenant id is read from the token\
  \ claims). 401 when invalid\n    or expired.\n  docs: https://docs.algovoi.co.uk/agent-session-auth\n- id: mandate-jwt\n  type: http\n  scheme: bearer\n  header: Authorization\n  applies_to: 'POST /mandate/pay (mandate_pay_mandate_pay_post)'\n  description: A mandate JWT is passed as a standard HTTP Bearer token; no X-Tenant-Id — mandate tokens are cross-tenant.\n- id: x402-payment\n  type: payment\n  protocol: x402 (v2 on pay.algovoi.co.uk; v1 and v2 on api.algovoi.co.uk)\n  header: X-PAYMENT\n  challenge: 'HTTP 402 with a JSON accepts[] body and a base64 payment-required header; on the pay rail every 402 carries one accept per enabled lane with payTo, amount (10000 micro-USDC) and a 1800-second payment_reference challenge token'\n  applies_to: 'pay.algovoi.co.uk /pay/v1/* (payment is the only credential), api.algovoi.co.uk /mpp/probe, /mpp/{resource_id}, /protected/{resource_id}, /r/{tenant}/{resource}, and mcp.algovoi.co.uk/mcp tool calls'\n  description: >-\n    \"No API key/bearer.\
  \ Each paid skill returns an x402 v2 402 challenge ... pay the USDC amount to payTo on your\n    chosen lane, bound per that lane's scheme, then resubmit with the X-PAYMENT proof.\" Mined-tx lanes (Algorand,\n    Voi, Stellar, Hedera, Solana, Tempo) weld the challenge into the tx note/memo/reference; EVM EIP-3009 lanes\n    (Base, Monad, Polygon, Arbitrum, OP, Arc) accept a stock signed TransferWithAuthorization with an optional nonce\n    weld. A2A over the same rail uses the a2a-x402 extension (payment-required task state).\n  observed: 'GET https://pay.algovoi.co.uk/pay/v1/verify/receipt → 402, 13,977-byte accepts[] body, payment-required header; POST tools/list on mcp.algovoi.co.uk/mcp → 402 x402 v1 challenge'\n  docs: https://docs.algovoi.co.uk/algovoi-pay\n- id: mpp-payment\n  type: payment\n  protocol: MPP (Machine Payments Protocol) — HTTP \"Payment\" authentication scheme\n  header: 'WWW-Authenticate: Payment (challenge) / PAYMENT-SIGNATURE (proof, declared as a header parameter\
  \ in the gateway spec)'\n  applies_to: 'api.algovoi.co.uk /mpp/* and /mpp/sub/*'\n  observed: 'GET https://api.algovoi.co.uk/mpp/probe → 402 with WWW-Authenticate: Payment realm=\"api.algovoi.co.uk\", id=\"algovoi-mpp-probe-static-v1\", method=\"tempo\", intent=\"charge\", expires=..., request=<base64>'\n- id: webhook-signature\n  type: hmac\n  header: X-AlgoVoi-Signature\n  key_prefix: algvw_\n  algorithm: 'HMAC-SHA256 over \"{t}.{raw_body}\"; header format t={unix_ts},v1={hex}; ±300 s tolerance; constant-time compare; 30-day dual-secret rotation window'\n  direction: inbound to the tenant (AlgoVoi signs outbound webhooks)\n  docs: https://docs.algovoi.co.uk/integrations/outbound-webhooks\n- id: reputation-credentials\n  type: apiKey\n  in: header\n  name: X-ATB-Credential / X-ATB-ZK-Credential\n  applies_to: 'Optional on payment-gated gateway operations (declared as header parameters); presenting a valid Falcon-1024 or Bulletproofs ATB Pass Certificate earns a 20% discount on the challenge\
  \ amount'\n  docs: https://docs.algovoi.co.uk/atb-reputation-credential\n- id: anonymous\n  type: none\n  applies_to: 'agents.algovoi.co.uk (clinic REST, A2A and MCP), verify.algovoi.co.uk (audit verifier), agent-trust-bench.algovoi.co.uk (/freebie, /discovery/resources, /stats.json; profiles answer 402), pay.algovoi.co.uk free tiers (/v1/receipt/verify 120/min, /verify/rfc9421 60/min), api.algovoi.co.uk /health, /compliance/attestation, /discovery/resources, /.well-known/*'\n  description: Public, no credential; abuse control is per-IP rate limiting.\nper_api:\n  algovoi-pay-payable-core-api: [x402-payment, anonymous]\n  algovoi-gateway-api: [tenant-api-key, admin-control-plane-key, agent-session-token, mandate-jwt, x402-payment, mpp-payment, reputation-credentials, webhook-signature]\n  algovoi-rfc9421-clinic-api: [anonymous]\n  algovoi-agent-trust-bench-api: [anonymous, x402-payment]\n  algovoi-audit-verifier-api: [anonymous]\n  algovoi-mcp-server: [anonymous (agents.algovoi.co.uk/mcp),\
  \ x402-payment (mcp.algovoi.co.uk/mcp), tenant-api-key (stdio package via ALGOVOI_API_KEY)]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/authentication/algovoi-co-uk-authentication.yml
summary_line: http-bearer/apiKey(header)/payment-as-auth(x402)/payment-as-auth(mpp)/hmac-webhook-signature/session-token/none · 9 schemes
tags:
- Payments
- Agentic Commerce
- x402
- A2A
- MCP
- Stablecoins
- Cryptocurrency
- Blockchain
- Compliance
- Digital Signature
- Post-Quantum Cryptography
- Verification
- Fintech
- Agent-Native
- Algorand
- United Kingdom
---
