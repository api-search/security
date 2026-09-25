---
anonymous_access: true
api_key_in: []
api_specs:
- filename: xguardgate-com-openapi.json
  format: json
  label: XGuard Universal Paid AI Agent + Secretless Gateway API
  slug: xguard-universal-paid-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xguardgate-com/refs/heads/main/openapi/xguardgate-com-openapi.json
- filename: xguardgate-com-reconcile-openapi.json
  format: json
  label: XGuard Reconcile API
  slug: xguard-reconcile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xguardgate-com/refs/heads/main/openapi/xguardgate-com-reconcile-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Xguardgate Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: XGuard declares 8 security scheme(s) across its OpenAPI definitions.
provider_name: XGuard
provider_slug: xguardgate-com
scheme_count: 8
schemes:
- applies_to:
  - xguardExecute with intent:demo or html
  - GET /v1/capabilities
  - GET /v1/pricing
  - POST /v1/pricing/quote
  - POST /v1/preflight
  - POST /v1/test
  - GET /supported
  - GET /healthz
  - every /.well-known document
  - MCP initialize and tools/list
  - A2A card
  evidence: 'Live 2026-09-19: POST /v1/execute {"intent":"demo"} -> 200 with no credential; POST /v1/pricing/quote -> 200; POST /mcp tools/list -> 200. Homepage: "No account. No API key. Pay only when you request live source execution."'
  id: anonymous
  type: none
- applies_to:
  - xguardExecute for web-extraction / product-offers / feed-digest
  - POST /v1/tools/web.fetch
  - POST /v1/tools/web.fetch/testnet
  - A2A skills (SendMessage)
  - MCP xguard_execute (challenge in the tool result; retry with params._meta["x402/payment"])
  docs: https://xguardgate.com/developers
  evidence: 'openapi xguardExecute: header params X-XGuard-Quote, Payment-Signature, X-XGuard-Credit; 402 response headers Payment-Required + X-XGuard-Quote; description "An unsigned request only returns a price; it does not fetch sources or settle payment." Live 402 observed 2026-09-19 with accepts[{scheme exact, network eip155:8453, asset 0x8335...2913, payTo 0x4f32...ba07}].'
  headers:
    challenge:
    - Payment-Required
    - X-XGuard-Quote
    - x-xguard-payment-identifier
    request:
    - Payment-Signature
    - X-XGuard-Quote
    response:
    - Payment-Response
    - x-xguard-receipt
    - x-xguard-proof
  id: x402-payment
  networks:
    production: eip155:8453 (Base)
    test: eip155:84532 (Base Sepolia), testnet:true
  principal: the paying wallet (Base USDC, EIP-3009 authorization); no account is created
  type: payment (x402 v2, HTTP 402 challenge/response)
- applies_to:
  - POST /v1/egress/credentials
  - GET /v1/egress/credentials
  - POST /v1/egress/capabilities
  - DELETE /v1/egress/capabilities/{id} (declared required in the spec)
  - POST /v1/actions/permits
  - GET /v1/balance
  - GET /v1/ledger
  docs: https://github.com/moelayyan90/XGuard/blob/main/docs/secretless-outcomes.md
  errors:
    401:
    - xguard_key_required
    - missing_xguard_license
  evidence: 'Live 2026-09-19: GET /v1/egress/credentials -> 401 {"error":{"code":"xguard_key_required",...}}; GET /v1/balance -> 401 missing_xguard_license; no WWW-Authenticate header. ai-plugin.json auth.authorization_type: "Operator management uses X-XGuard-Key".'
  how_obtained: Issued with Operator Usage Credits (JOD 3.550 / 5,000 credits, Lemon Squeezy checkout at https://xguardgate.com/pricing/operator). The issuance flow itself is not documented publicly; the site warns "Do not place an operator key in an AI prompt."
  id: xguard-key
  in: header
  name: X-XGuard-Key
  role: operator
  storage: Provider stores only an irreversible hash of the key (privacy page).
  type: apiKey
- applies_to:
  - POST /v1/egress/fetch
  errors:
    401: capability_required
    402: budget exceeded before billing
    403: capability or credential scope denied
  evidence: 'ai-plugin.json auth.authorization_type: "agent egress uses a scoped xgc_ capability"; /.well-known/xguard-egress.json security_model: "operator holds reusable secret; agent receives scoped short-lived XGuard capability".'
  id: scoped-capability
  issued_by: POST /v1/egress/capabilities (operator, X-XGuard-Key) with credential_id, target_origin, path_prefix, allowed_methods, ttl_seconds 30-3600, max_calls, max_total_credits, max_credits_per_call
  prefix: xgc_
  revoked_by: DELETE /v1/egress/capabilities/{id}
  role: agent (delegated)
  sdk: createXGuardAgentClient(process.env.XGUARD_CAPABILITY) in sdk/index.js
  type: capability token (bearer-like, passed in the JSON body field `capability`)
- applies_to:
  - GET /v1/results/{payment_identifier} (declared required in the spec)
  - MCP xguard_get_result
  evidence: 'llms.txt Recovery: "This quote grants access to the stored public-source result; do not publish it." README: "treat that quote as a private bearer token." 403 "Unsafe target or recovery credential" on mismatch.'
  id: recovery-quote
  type: bearer (signed ES256 JWS quote, header X-XGuard-Quote)
- applies_to:
  - xguardExecute retry after 502 'No usable source; execution credit retained'
  evidence: 'openapi xguardExecute header param X-XGuard-Credit; pricing page: "the response provides an execution credit for the same outcome."'
  id: execution-credit
  type: signed credential (header X-XGuard-Credit)
- applies_to:
  - POST /v1/actions/execute
  evidence: /.well-known/xguard-actions.json controls list.
  id: action-permit
  issued_by: POST /v1/actions/permits (X-XGuard-Key; 428 if no mandate)
  public_key: https://api.xguardgate.com/.well-known/xguard-actions-key.json
  type: signed single-use permit (ES256) bound to a mandate
- applies_to:
  - POST /edge/{merchant-host}/{path}
  errors:
    403: Merchant hostname has not authorized XGuard Edge
  evidence: /docs edge.merchant_authorization; /healthz universal_edge.
  id: merchant-dns-authorization
  record: _xguard.<merchant-host> TXT "xguard-edge=enabled"
  type: domain-control proof (DNS TXT), not a credential
slug: xguardgate-com-authentication
source_filename: xguardgate-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://xguardgate.com/.well-known/ai-plugin.json\nderived_from: openapi/xguardgate-com-openapi.json\nprobed: true\ndocs:\n- https://xguardgate.com/developers\n- https://github.com/moelayyan90/XGuard/blob/main/docs/secretless-outcomes.md\n- https://api.xguardgate.com/.well-known/oauth-protected-resource\n- https://api.xguardgate.com/.well-known/xguard-egress.json\nsummary: >-\n  XGuard has no user accounts, no API-key signup and no OAuth. The OpenAPI declares NO securitySchemes (a\n  contract-quality gap - the credentials exist only as header parameters and prose; overlays/ proposes four\n  schemes), and the RFC 9728 documents on both the API and MCP resources say so plainly: bearer_methods_supported\n  [], oauth_supported false, \"Public discovery and pay-per-request tools do not require an XGuard account or\n  OAuth bearer token.\" Authorization is layered by role instead. Anyone may discover, preview and quote. A PAID\n\
  \  outcome is authorised by an x402 v2 payment - the retry of a 402 carries Payment-Signature and the preserved\n  signed quote - so the wallet, not an account, is the principal. An OPERATOR who buys Usage Credits gets an\n  X-XGuard-Key (stored server-side only as an irreversible hash) for credential custody, capability issuance and\n  Action Rail permits; an AGENT acting for that operator receives a short-lived scoped capability (xgc_...) and\n  never the upstream secret. Recovery of a paid result uses the original quote as a bearer token, and a signed\n  execution credit (X-XGuard-Credit) redeems a failed paid execution. Merchant hosts authorise the Edge proxy by\n  publishing a DNS TXT record rather than by any key.\nschemes:\n- id: anonymous\n  type: none\n  applies_to: [xguardExecute with intent:demo or html, 'GET /v1/capabilities', 'GET /v1/pricing', 'POST /v1/pricing/quote', 'POST /v1/preflight', 'POST /v1/test', 'GET /supported', 'GET /healthz', every /.well-known document, MCP\
  \ initialize and tools/list, A2A card]\n  evidence: 'Live 2026-09-19: POST /v1/execute {\"intent\":\"demo\"} -> 200 with no credential; POST /v1/pricing/quote -> 200; POST /mcp tools/list -> 200. Homepage: \"No account. No API key. Pay only when you request live source execution.\"'\n- id: x402-payment\n  type: payment (x402 v2, HTTP 402 challenge/response)\n  headers:\n    challenge: [Payment-Required, X-XGuard-Quote, x-xguard-payment-identifier]\n    request: [Payment-Signature, X-XGuard-Quote]\n    response: [Payment-Response, x-xguard-receipt, x-xguard-proof]\n  principal: the paying wallet (Base USDC, EIP-3009 authorization); no account is created\n  applies_to:\n  - xguardExecute for web-extraction / product-offers / feed-digest\n  - 'POST /v1/tools/web.fetch'\n  - 'POST /v1/tools/web.fetch/testnet'\n  - A2A skills (SendMessage)\n  - 'MCP xguard_execute (challenge in the tool result; retry with params._meta[\"x402/payment\"])'\n  networks: {production: 'eip155:8453 (Base)', test:\
  \ 'eip155:84532 (Base Sepolia), testnet:true'}\n  evidence: 'openapi xguardExecute: header params X-XGuard-Quote, Payment-Signature, X-XGuard-Credit; 402 response headers Payment-Required + X-XGuard-Quote; description \"An unsigned request only returns a price; it does not fetch sources or settle payment.\" Live 402 observed 2026-09-19 with accepts[{scheme exact, network eip155:8453, asset 0x8335...2913, payTo 0x4f32...ba07}].'\n  docs: https://xguardgate.com/developers\n- id: xguard-key\n  type: apiKey\n  in: header\n  name: X-XGuard-Key\n  role: operator\n  applies_to: ['POST /v1/egress/credentials', 'GET /v1/egress/credentials', 'POST /v1/egress/capabilities', 'DELETE /v1/egress/capabilities/{id} (declared required in the spec)', 'POST /v1/actions/permits', 'GET /v1/balance', 'GET /v1/ledger']\n  how_obtained: 'Issued with Operator Usage Credits (JOD 3.550 / 5,000 credits, Lemon Squeezy checkout at https://xguardgate.com/pricing/operator). The issuance flow itself is not documented\
  \ publicly; the site warns \"Do not place an operator key in an AI prompt.\"'\n  storage: 'Provider stores only an irreversible hash of the key (privacy page).'\n  errors: {401: [xguard_key_required, missing_xguard_license]}\n  evidence: 'Live 2026-09-19: GET /v1/egress/credentials -> 401 {\"error\":{\"code\":\"xguard_key_required\",...}}; GET /v1/balance -> 401 missing_xguard_license; no WWW-Authenticate header. ai-plugin.json auth.authorization_type: \"Operator management uses X-XGuard-Key\".'\n  docs: https://github.com/moelayyan90/XGuard/blob/main/docs/secretless-outcomes.md\n- id: scoped-capability\n  type: capability token (bearer-like, passed in the JSON body field `capability`)\n  prefix: xgc_\n  role: agent (delegated)\n  applies_to: ['POST /v1/egress/fetch']\n  issued_by: 'POST /v1/egress/capabilities (operator, X-XGuard-Key) with credential_id, target_origin, path_prefix, allowed_methods, ttl_seconds 30-3600, max_calls, max_total_credits, max_credits_per_call'\n  revoked_by:\
  \ 'DELETE /v1/egress/capabilities/{id}'\n  sdk: 'createXGuardAgentClient(process.env.XGUARD_CAPABILITY) in sdk/index.js'\n  errors: {401: capability_required, 403: 'capability or credential scope denied', 402: 'budget exceeded before billing'}\n  evidence: 'ai-plugin.json auth.authorization_type: \"agent egress uses a scoped xgc_ capability\"; /.well-known/xguard-egress.json security_model: \"operator holds reusable secret; agent receives scoped short-lived XGuard capability\".'\n- id: recovery-quote\n  type: bearer (signed ES256 JWS quote, header X-XGuard-Quote)\n  applies_to: ['GET /v1/results/{payment_identifier} (declared required in the spec)', MCP xguard_get_result]\n  evidence: 'llms.txt Recovery: \"This quote grants access to the stored public-source result; do not publish it.\" README: \"treat that quote as a private bearer token.\" 403 \"Unsafe target or recovery credential\" on mismatch.'\n- id: execution-credit\n  type: signed credential (header X-XGuard-Credit)\n  applies_to:\
  \ [xguardExecute retry after 502 'No usable source; execution credit retained']\n  evidence: 'openapi xguardExecute header param X-XGuard-Credit; pricing page: \"the response provides an execution credit for the same outcome.\"'\n- id: action-permit\n  type: signed single-use permit (ES256) bound to a mandate\n  applies_to: ['POST /v1/actions/execute']\n  issued_by: 'POST /v1/actions/permits (X-XGuard-Key; 428 if no mandate)'\n  public_key: https://api.xguardgate.com/.well-known/xguard-actions-key.json\n  evidence: /.well-known/xguard-actions.json controls list.\n- id: merchant-dns-authorization\n  type: domain-control proof (DNS TXT), not a credential\n  applies_to: ['POST /edge/{merchant-host}/{path}']\n  record: '_xguard.<merchant-host> TXT \"xguard-edge=enabled\"'\n  errors: {403: 'Merchant hostname has not authorized XGuard Edge'}\n  evidence: /docs edge.merchant_authorization; /healthz universal_edge.\noauth2: false\nopenid_connect: false\nprotected_resource_metadata:\n  api: well-known/xguardgate-com-oauth-protected-resource.json\n\
  \  mcp: well-known/xguardgate-com-oauth-protected-resource-mcp.json\n  authorization_servers: []\n  note: 'Served and truthful: they document that there is no OAuth. /.well-known/oauth-authorization-server returns a deliberate 404 (\"XGuard does not advertise a fictitious OAuth issuer\").'\nspec_gaps:\n- No components.securitySchemes and no security requirements in the OpenAPI, so a generated client cannot know which operations need X-XGuard-Key or a capability without reading the prose; proposed schemes are in overlays/xguardgate-com-openapi-overlay.yaml.\n- 401 responses carry no WWW-Authenticate header.\nkey_hygiene:\n- 'Never enter a wallet private key into the site or an AI conversation (developers page); XGUARD_PAYER_PRIVATE_KEY stays in the local process environment.'\n- 'Do not place an operator key in an AI prompt (pricing/operator page).'\n- 'Agents receive capabilities, never upstream secrets; the response filter blocks literal, encoded and base64 credential reflections (docs/secretless-outcomes.md).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xguardgate-com/refs/heads/main/authentication/xguardgate-com-authentication.yml
summary_line: 8 schemes
tags:
- Agents
- Agentic Commerce
- x402
- MCP
- A2A
- Micropayments
- Web Extraction
- Feed Aggregation
- Credential Broker
- API Gateway
- Agent Security
- Agent-Native
---
