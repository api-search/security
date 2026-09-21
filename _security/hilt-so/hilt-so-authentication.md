---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hilt-so-openapi.yml
  format: yaml
  label: Hilt API (Pay API + Workspace)
  slug: hilt-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/openapi/hilt-so-openapi.yml
- filename: hilt-so-transaction-evidence-openapi.yml
  format: yaml
  label: Hilt Solana Transaction Evidence API
  slug: transaction-evidence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/openapi/hilt-so-transaction-evidence-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Hilt So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hilt declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Hilt
provider_slug: hilt-so
scheme_count: 6
schemes:
- applies_to: Workspace merchant routes (/v1/products, /v1/memberships, /v1/receipts, /v1/support, /v1/testing) and Hilt Pay API routes (/v1/access/*)
  header: X-Hilt-Key
  in: header
  key_prefixes:
    live: hk_live_
    sandbox: hk_sandbox_
  management: Dashboard -> Advanced; GET/POST /v1/keys, DELETE /v1/keys/{key_id}; CLI hilt keys *. Raw key shown once; rotation = create replacement, deploy, GET /v1/products to confirm, revoke old.
  name: HiltApiKey
  permissions:
  - access:read - check entitlements and read Pay API rails
  - access:write - create Pay API apps, products, and payment sessions
  - access:webhooks - register webhook endpoints for Pay API flows
  type: apiKey
  unauthenticated_response:
    body: '{"detail":"Authentication required"}'
    probed: GET /v1/account/me and POST /v1/access/entitlements/consume, 2026-09-19
    status: 401
- applies_to: 'Dashboard/session routes: /v1/auth/*, /v1/account/*, /v1/webhooks/endpoints (quickstart uses Bearer for webhook endpoint creation and test events), /v1/keys, /v1/billing/*'
  header: 'Authorization: Bearer <token>'
  name: DashboardBearer
  note: Postman environment variable bearerToken.
  obtain: POST /v1/auth/login, POST /v1/auth/wallet (wallet-signature login), /v1/auth/oauth/{provider}/start; refresh via POST /v1/auth/refresh; CLI hilt login
  scheme: bearer
  type: http
- authorizationUrl: https://api.hilt.so/oauth/authorize
  client_auth: none (public clients)
  discovery: well-known/hilt-so-api-oauth-authorization-server.json
  flow: authorizationCode
  identity: Sign in with X supplies the PayMe identity
  name: PayMeOAuth
  pkce: S256 required
  refresh: refresh_token grant supported
  registrationUrl: https://api.hilt.so/oauth/register (RFC 7591 dynamic client registration)
  resource: https://api.hilt.so/mcp/pay-me (RFC 9728 metadata at /.well-known/oauth-protected-resource/mcp/pay-me)
  revocationUrl: https://api.hilt.so/oauth/revoke
  scopes:
    pay_me:prepare: Start and manage wallet-approved payments to verified PayMe handles
    pay_me:read: Read connector-started payments and received activity
    pay_me:request: Create and manage self-shared payment links
  tokenUrl: https://api.hilt.so/oauth/token
  type: oauth2
- applies_to: Merchant-protected resources; Hilt agent-commerce plan activation; the transaction-evidence resource (0.05 USDC/request); paid MCP gateway tools
  headers:
    challenge: PAYMENT-REQUIRED (HTTP 402 response; base64 payment requirement)
    proof: PAYMENT-SIGNATURE (request header on retry; declared as a header parameter on POST /v1/access/x402/settle and on /v1/solana/transaction-evidence)
    result: PAYMENT-RESPONSE (response header after settlement)
  name: x402PaymentSignature
  note: 'Not a credential for Hilt itself: the buyer never receives the merchant X-Hilt-Key.'
  protocol: x402 V2
  settlement: Solana USDC (network solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp per the agent-commerce offer)
  type: payment-protocol
- applies_to: MPP metered session channels (/v1/access/metered-sessions/*) and the public PayMe agent payment action POST /v1/pay-me/payments (no payer account, OAuth grant or API key)
  headers:
    challenge: 'WWW-Authenticate: Payment'
    credential: 'Authorization: Payment <MPP credential>'
    receipt: Payment-Receipt (successful responses)
  name: MPPPaymentCredential
  on_chain_program: CHNLxYvVA28MJP9PrFuDXccuoGXAx7jBacfLEkahyGsX (Solana mainnet channel program)
  protocol: Machine Payments Protocol (MPP) over HTTP 402
  type: payment-protocol
- algorithm: HMAC-SHA256 with the endpoint signing secret
  also: Stripe-Signature header parameter on POST /v1/billing/webhooks/stripe (Hilt account billing inbound from Stripe)
  direction: Hilt -> merchant (verify inbound webhooks)
  format: t=<unix_timestamp>,v1=<hex_hmac_sha256>
  header: X-Hilt-Signature
  name: WebhookSignature
  signed_payload: <timestamp>.<raw_json_body>
  type: hmac
slug: hilt-so-authentication
source_filename: hilt-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://docs.hilt.so/developers/api-keys; https://docs.hilt.so/developers/access; https://docs.hilt.so/developers/quickstart;\n  https://docs.hilt.so/developers/payment-channels; https://api.hilt.so/.well-known/oauth-authorization-server (probed);\n  openapi/hilt-so-openapi.yml (header parameters)\ndocs: https://docs.hilt.so/developers/api-keys\nspec_gap: The published OpenAPI declares NO components.securitySchemes and no security requirements on any of its\n  165 operations; every scheme below is documented in prose or discoverable from RFC 8414/9728 metadata. derive-authentication.py\n  therefore produced nothing and this profile is hand-built from the docs.\nschemes:\n- name: HiltApiKey\n  type: apiKey\n  in: header\n  header: X-Hilt-Key\n  key_prefixes:\n    live: hk_live_\n    sandbox: hk_sandbox_\n  applies_to: Workspace merchant routes (/v1/products, /v1/memberships, /v1/receipts, /v1/support, /v1/testing)\n    and Hilt\
  \ Pay API routes (/v1/access/*)\n  permissions:\n  - access:read - check entitlements and read Pay API rails\n  - access:write - create Pay API apps, products, and payment sessions\n  - access:webhooks - register webhook endpoints for Pay API flows\n  management: Dashboard -> Advanced; GET/POST /v1/keys, DELETE /v1/keys/{key_id}; CLI hilt keys *. Raw key shown\n    once; rotation = create replacement, deploy, GET /v1/products to confirm, revoke old.\n  unauthenticated_response:\n    status: 401\n    body: '{\"detail\":\"Authentication required\"}'\n    probed: GET /v1/account/me and POST /v1/access/entitlements/consume, 2026-09-19\n- name: DashboardBearer\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <token>'\n  applies_to: 'Dashboard/session routes: /v1/auth/*, /v1/account/*, /v1/webhooks/endpoints (quickstart uses Bearer\n    for webhook endpoint creation and test events), /v1/keys, /v1/billing/*'\n  obtain: POST /v1/auth/login, POST /v1/auth/wallet (wallet-signature\
  \ login), /v1/auth/oauth/{provider}/start; refresh\n    via POST /v1/auth/refresh; CLI hilt login\n  note: Postman environment variable bearerToken.\n- name: PayMeOAuth\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256 required\n  authorizationUrl: https://api.hilt.so/oauth/authorize\n  tokenUrl: https://api.hilt.so/oauth/token\n  registrationUrl: https://api.hilt.so/oauth/register (RFC 7591 dynamic client registration)\n  revocationUrl: https://api.hilt.so/oauth/revoke\n  refresh: refresh_token grant supported\n  client_auth: none (public clients)\n  scopes:\n    pay_me:read: Read connector-started payments and received activity\n    pay_me:request: Create and manage self-shared payment links\n    pay_me:prepare: Start and manage wallet-approved payments to verified PayMe handles\n  resource: https://api.hilt.so/mcp/pay-me (RFC 9728 metadata at /.well-known/oauth-protected-resource/mcp/pay-me)\n  identity: Sign in with X supplies the PayMe identity\n  discovery: well-known/hilt-so-api-oauth-authorization-server.json\n\
  - name: x402PaymentSignature\n  type: payment-protocol\n  protocol: x402 V2\n  headers:\n    challenge: PAYMENT-REQUIRED (HTTP 402 response; base64 payment requirement)\n    proof: PAYMENT-SIGNATURE (request header on retry; declared as a header parameter on POST /v1/access/x402/settle\n      and on /v1/solana/transaction-evidence)\n    result: PAYMENT-RESPONSE (response header after settlement)\n  settlement: Solana USDC (network solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp per the agent-commerce offer)\n  applies_to: Merchant-protected resources; Hilt agent-commerce plan activation; the transaction-evidence resource\n    (0.05 USDC/request); paid MCP gateway tools\n  note: 'Not a credential for Hilt itself: the buyer never receives the merchant X-Hilt-Key.'\n- name: MPPPaymentCredential\n  type: payment-protocol\n  protocol: Machine Payments Protocol (MPP) over HTTP 402\n  headers:\n    challenge: 'WWW-Authenticate: Payment'\n    credential: 'Authorization: Payment <MPP credential>'\n   \
  \ receipt: Payment-Receipt (successful responses)\n  applies_to: MPP metered session channels (/v1/access/metered-sessions/*) and the public PayMe agent payment action\n    POST /v1/pay-me/payments (no payer account, OAuth grant or API key)\n  on_chain_program: CHNLxYvVA28MJP9PrFuDXccuoGXAx7jBacfLEkahyGsX (Solana mainnet channel program)\n- name: WebhookSignature\n  type: hmac\n  header: X-Hilt-Signature\n  format: t=<unix_timestamp>,v1=<hex_hmac_sha256>\n  signed_payload: <timestamp>.<raw_json_body>\n  algorithm: HMAC-SHA256 with the endpoint signing secret\n  direction: Hilt -> merchant (verify inbound webhooks)\n  also: Stripe-Signature header parameter on POST /v1/billing/webhooks/stripe (Hilt account billing inbound from\n    Stripe)\nrequest_id_headers:\n- X-Hilt-Request-Id\n- X-Request-Id\nsummary: API key (X-Hilt-Key, hk_live_/hk_sandbox_) for merchants and Pay API; bearer session tokens for the dashboard\n  surface; OAuth 2.1-style PKCE with DCR for the PayMe MCP connector; x402\
  \ V2 and MPP payment credentials for paid\n  requests; HMAC-signed webhooks.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/authentication/hilt-so-authentication.yml
summary_line: 6 schemes
tags:
- Payments
- Solana
- Stablecoins
- USDC
- Crypto Payments
- Agentic Payments
- x402
- Checkout
- Subscription
- Webhook
- MCP
- Entitlements
- Micropayments
- Developer Tools
- Fintech
---
